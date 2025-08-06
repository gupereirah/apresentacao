<script>
	import { onMount } from 'svelte';
	import { Fireworks } from 'fireworks-js';
	
	export let isActive = false;
	
	let showTitle = false;
	let showTypingMessage = false;
	let showFireworks = false;
	let fireworksContainer;
	let fireworksInstance;
	let typedText = '';
	let isTyping = false;
	let animationStarted = false;
	
	const fullMessage = "Apenas mais uma informação para vocês, essa apresentação também foi feita utilizando ferramentas de IA para Devs";
	const typingSpeed = 80; // milliseconds per character
	
	onMount(() => {
		if (isActive) {
			startAnimation();
		}
	});
	
	$: if (isActive && !animationStarted) {
		startAnimation();
	} else if (!isActive) {
		// Para os fogos e reset quando sair do slide
		if (fireworksInstance) {
			fireworksInstance.stop();
		}
		resetAnimation();
	}
	
	function startAnimation() {
		animationStarted = true;
		setTimeout(() => {
			showTypingMessage = true;
			startTyping();
		}, 500);
	}
	
	function resetAnimation() {
		showTitle = false;
		showTypingMessage = false;
		showFireworks = false;
		typedText = '';
		isTyping = false;
		animationStarted = false;
		if (fireworksInstance) {
			fireworksInstance.stop();
			fireworksInstance = null;
		}
	}
	
	function startTyping() {
		isTyping = true;
		typedText = '';
		let currentIndex = 0;
		
		const typeInterval = setInterval(() => {
			if (currentIndex < fullMessage.length) {
				typedText = fullMessage.substring(0, currentIndex + 1);
				currentIndex++;
			} else {
				isTyping = false;
				clearInterval(typeInterval);
				// Mostra o título "Obrigado" após terminar de digitar
				setTimeout(() => {
					showTitle = true;
				}, 1000);
				// Inicia os fogos após o título aparecer
				setTimeout(() => {
					showFireworks = true;
					startFireworks();
				}, 2500);
			}
		}, typingSpeed);
	}
	
	function startFireworks() {
		if (fireworksContainer && !fireworksInstance) {
			const containerHeight = fireworksContainer.clientHeight;
			const containerWidth = fireworksContainer.clientWidth;
			
			fireworksInstance = new Fireworks(fireworksContainer, {
				hue: { min: 0, max: 360 },
				delay: { min: 20, max: 40 },
				rocketsPoint: { min: 70, max: 80 },
				opacity: 0.8,
				acceleration: 1.02,
				friction: 0.97,
				gravity: 1.2,
				particles: 80,
				trace: 4,
				explosion: 8,
				boundaries: {
					x: 0,
					y: 0,
					width: containerWidth,
					height: containerHeight
				},
				sound: {
					enabled: false
				},
				mouse: {
					click: false,
					move: false,
					max: 0
				}
			});
			fireworksInstance.start();
		}
	}
</script>

<div class="slide-content">
	<!-- Título animado -->
	<div class="title-container" class:show={showTitle}>
		<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white drop-shadow-2xl px-4">
			🎉 Obrigado!
		</h1>
	</div>
	
	<!-- Mensagem com efeito de digitação -->
	<div class="typing-message-container" class:show={showTypingMessage}>
		<div class="message-box">
			<div class="message-text">
				{typedText}<span class="cursor" class:blinking={isTyping}>|</span>
			</div>
		</div>
	</div>
	
	<!-- Fogos de Artifício -->
	<div 
		bind:this={fireworksContainer}
		class="fireworks-container" 
		class:show={showFireworks}
	></div>
</div>

<style>
	.slide-content {
		text-align: center;
		display: flex;
		flex-direction: column;
		position: relative;
		overflow: hidden;
		width: 100%;
		height: 80vh;
		background: linear-gradient(135deg, #1a1a2e 0%, #16213e 30%, #0f3460 60%, #0a1930 100%);
		min-height: 100vh;
		justify-content: center;
		padding: 2rem 1rem;
	}
	
	.title-container {
		opacity: 0;
		transform: translateY(-30px);
		transition: all 0.8s ease-out;
		position: absolute;
		top: 3rem;
		left: 0;
		right: 0;
		z-index: 10;
	}
	
	.typing-message-container {
		opacity: 0;
		transform: translateY(30px);
		transition: all 1s ease-out;
		flex: 1;
		display: flex;
		align-items: center;
		justify-content: center;
		position: relative;
		padding: 1rem;
	}
	
	.fireworks-container {
		opacity: 0;
		transform: translateY(30px);
		transition: all 0.8s ease-out;
	}
	
	.title-container.show,
	.typing-message-container.show,
	.fireworks-container.show {
		opacity: 1;
		transform: scale(1) translateX(0) translateY(0);
	}
	
	/* Estilos da mensagem com efeito de digitação */
	.message-box {
		background: linear-gradient(145deg, rgba(0, 20, 40, 0.95), rgba(0, 40, 80, 0.9));
		border: 2px solid rgba(100, 200, 255, 0.6);
		border-radius: 20px;
		padding: 2rem 2.5rem;
		backdrop-filter: blur(15px);
		box-shadow: 0 0 40px rgba(100, 200, 255, 0.4);
		max-width: 90%;
		position: relative;
		animation: messageGlow 3s ease-in-out infinite alternate;
	}
	
			.message-text {
			font-size: 1.5rem;
		color: rgba(255, 255, 255, 0.95);
		font-weight: 500;
		line-height: 1.6;
		text-shadow: 0 0 15px rgba(100, 200, 255, 0.6);
		font-family: 'Monaco', 'Consolas', 'Courier New', monospace;
	}
	
	.cursor {
		display: inline-block;
		margin-left: 2px;
		color: rgba(100, 200, 255, 0.9);
		font-weight: bold;
		text-shadow: 0 0 10px rgba(100, 200, 255, 0.8);
	}
	
	.cursor.blinking {
		animation: cursorBlink 1s infinite;
	}
	
	.title-container.show h1 {
		animation: titleGlow 2s ease-in-out infinite alternate;
	}
	
	/* Container dos Fogos de Artifício */
	.fireworks-container {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		pointer-events: none;
		z-index: 1000;
		opacity: 0;
		transition: opacity 0.8s ease-out;
	}
	
	.fireworks-container.show {
		opacity: 1;
	}

	/* Animações */
	@keyframes titleGlow {
		from {
			text-shadow: 0 0 20px rgba(255, 255, 255, 0.5);
		}
		to {
			text-shadow: 0 0 40px rgba(255, 255, 255, 0.8), 0 0 60px rgba(147, 51, 234, 0.5);
		}
	}

	@keyframes messageGlow {
		0% { 
			box-shadow: 0 0 40px rgba(100, 200, 255, 0.4);
			border-color: rgba(100, 200, 255, 0.6);
		}
		100% { 
			box-shadow: 0 0 60px rgba(100, 200, 255, 0.7);
			border-color: rgba(100, 200, 255, 0.9);
		}
	}

	@keyframes cursorBlink {
		0%, 50% { 
			opacity: 1;
		}
		51%, 100% { 
			opacity: 0;
		}
	}
	
	/* Responsividade */
			@media (max-width: 768px) {
			.title-container {
				top: 2rem;
			}
			
			.message-box {
				padding: 1.5rem 2rem;
				max-width: 95%;
			}
			
			.message-text {
				font-size: 1.25rem;
			}
	}
	
	@media (max-width: 320px) {
		.slide-content h1 {
			font-size: 2rem !important;
		}
		
		.message-box {
			padding: 1rem 1.5rem;
		}
		
		.message-text {
			font-size: 0.875rem;
		}
	}
</style>