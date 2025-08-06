<script>
	import { onMount } from 'svelte';
	import { Fireworks } from 'fireworks-js';
	
	export let isActive = false;
	
	let showTitle = false;
	let showJarvis = false;
	let jarvisActivated = false;
	let showJarvisMessage = false;
	let showFireworks = false;
	let fireworksContainer;
	let fireworksInstance;
	
	onMount(() => {
		if (isActive) {
			startAnimation();
		}
	});
	
	$: if (isActive) {
		startAnimation();
	} else {
		// Para os fogos quando sair do slide
		if (fireworksInstance) {
			fireworksInstance.stop();
		}
	}
	
	function startAnimation() {
		setTimeout(() => showTitle = true, 500);
		setTimeout(() => {
			showJarvis = true;
		}, 2000);
		setTimeout(() => {
			jarvisActivated = true;
		}, 3000);
		setTimeout(() => {
			showJarvisMessage = true;
		}, 4500);
		setTimeout(() => {
			showFireworks = true;
			startFireworks();
		}, 7000);
	}
	
	function startFireworks() {
		if (fireworksContainer && !fireworksInstance) {
			const containerHeight = fireworksContainer.clientHeight;
			const containerWidth = fireworksContainer.clientWidth;
			
			fireworksInstance = new Fireworks(fireworksContainer, {
				hue: { min: 0, max: 360 },
				delay: { min: 20, max: 40 },
				rocketsPoint: { min: 70, max: 80 }, // Lança da altura do quadro
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
					height: containerHeight // Usa toda a altura da tela
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
		<h1 class="text-5xl font-bold text-white drop-shadow-2xl">
			🎉 Obrigado!
		</h1>
	</div>
	

	<!-- Holograma JARVIS -->
	<div class="jarvis-container" class:show={showJarvis} class:activated={jarvisActivated}>
		<!-- Holograma do Rosto -->
		<div class="hologram-face">
			<!-- Contorno da cabeça -->
			<div class="face-outline">
				<div class="scan-line"></div>
			</div>
			
			<!-- Rosto holográfico -->
			<div class="face-structure">
				<!-- Testa e linhas superiores -->
				<div class="forehead">
					<div class="brain-pattern">
						<div class="neural-dot dot-1"></div>
						<div class="neural-dot dot-2"></div>
						<div class="neural-dot dot-3"></div>
						<div class="neural-connection conn-1"></div>
						<div class="neural-connection conn-2"></div>
					</div>
				</div>
				
				<!-- Olhos holográficos -->
				<div class="eyes">
					<div class="eye left-eye">
						<div class="eye-core">
							<div class="iris"></div>
							<div class="pupil"></div>
						</div>
						<div class="eye-glow"></div>
						<div class="eye-scan"></div>
					</div>
					<div class="eye right-eye">
						<div class="eye-core">
							<div class="iris"></div>
							<div class="pupil"></div>
						</div>
						<div class="eye-glow"></div>
						<div class="eye-scan"></div>
					</div>
				</div>
				
				<!-- Nariz (linhas geométricas) -->
				<div class="nose">
					<div class="nose-line line-1"></div>
					<div class="nose-line line-2"></div>
				</div>
				
				<!-- Boca holográfica -->
				<div class="mouth">
					<div class="mouth-line"></div>
					<div class="mouth-glow"></div>
				</div>
				
				<!-- Mandíbula -->
				<div class="jawline">
					<div class="jaw-left"></div>
					<div class="jaw-right"></div>
				</div>
			</div>
			
			<!-- Grade holográfica -->
			<div class="hologram-grid">
				<div class="grid-line horizontal h-1"></div>
				<div class="grid-line horizontal h-2"></div>
				<div class="grid-line horizontal h-3"></div>
				<div class="grid-line horizontal h-4"></div>
				<div class="grid-line horizontal h-5"></div>
				<div class="grid-line vertical v-1"></div>
				<div class="grid-line vertical v-2"></div>
				<div class="grid-line vertical v-3"></div>
				<div class="grid-line vertical v-4"></div>
			</div>
			
			<!-- Efeitos de interferência */
			<div class="interference">
				<div class="glitch-line g-1"></div>
				<div class="glitch-line g-2"></div>
				<div class="glitch-line g-3"></div>
			</div>
			
			<!-- Partículas flutuantes */
			<div class="floating-particles">
				<div class="particle p-1"></div>
				<div class="particle p-2"></div>
				<div class="particle p-3"></div>
				<div class="particle p-4"></div>
				<div class="particle p-5"></div>
				<div class="particle p-6"></div>
			</div>
		</div>
	</div>
	
	<!-- Mensagem do JARVIS embaixo -->
	<div class="jarvis-message" class:show={showJarvisMessage}>
		<div class="message-container">
			<div class="typing-indicator">
				<span class="dot dot-1"></span>
				<span class="dot dot-2"></span>
				<span class="dot dot-3"></span>
			</div>
			<p class="message-text">
				Lembre-se... eu também fui feito por IA
			</p>
			<div class="message-signature">
				- Sistema de IA Avançado
			</div>
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
</div>

<style>
	.slide-content {
		text-align: center;
		display: flex;
		flex-direction: column;
		position: relative;
		overflow: hidden;
		width: 100%;
		height: 72vh;
		background: linear-gradient(135deg, #1a1a2e 0%, #16213e 30%, #0f3460 60%, #0a1930 100%);
	}
	
	.title-container {
		opacity: 0;
		transform: translateY(30px);
		transition: all 0.8s ease-out;
		position: absolute;
		top: 2rem;
		left: 0;
		right: 0;
		z-index: 10;
	}
	
	.jarvis-container {
		opacity: 0;
		transform: scale(0.3);
		transition: all 1.5s ease-out;
		flex: 1;
		display: flex;
		align-items: center;
		justify-content: center;
		margin-top: 4rem;
		position: relative;
	}
	
	.fireworks-container {
		opacity: 0;
		transform: translateY(30px);
		transition: all 0.8s ease-out;
	}
	
	.title-container.show,
	.jarvis-container.show,
	.fireworks-container.show {
		opacity: 1;
		transform: scale(1) translateX(0) translateY(0);
	}
	
	.jarvis-message {
		opacity: 0;
		transform: translateY(30px);
		transition: all 1s ease-out;
		position: absolute;
		bottom: 8rem;
		left: 50%;
		transform: translateX(-50%) translateY(30px);
		z-index: 5;
	}
	
	.jarvis-message.show {
		opacity: 1;
		transform: translateX(-50%) translateY(0);
	}
	
	.title-container.show h1 {
		animation: titleGlow 2s ease-in-out infinite alternate;
	}
	
	@keyframes titleGlow {
		from {
			text-shadow: 0 0 20px rgba(255, 255, 255, 0.5);
		}
		to {
			text-shadow: 0 0 40px rgba(255, 255, 255, 0.8), 0 0 60px rgba(147, 51, 234, 0.5);
		}
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

	/* Estilos do Holograma JARVIS */
	.hologram-face {
		width: 350px;
		height: 400px;
		position: relative;
		filter: drop-shadow(0 0 30px rgba(100, 200, 255, 0.6));
	}

	/* Contorno da cabeça */
	.face-outline {
		position: absolute;
		top: 0;
		left: 50%;
		transform: translateX(-50%);
		width: 200px;
		height: 250px;
		border: 2px solid rgba(100, 200, 255, 0.4);
		border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
		animation: outlineGlow 3s ease-in-out infinite alternate;
	}

	.scan-line {
		position: absolute;
		top: 0;
		left: 0;
		right: 0;
		height: 2px;
		background: linear-gradient(90deg, transparent, rgba(100, 200, 255, 0.8), transparent);
		animation: scanMove 2s ease-in-out infinite;
	}

	/* Estrutura do rosto */
	.face-structure {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 180px;
		height: 220px;
	}

	/* Testa com padrão neural */
	.forehead {
		position: absolute;
		top: 0;
		left: 50%;
		transform: translateX(-50%);
		width: 120px;
		height: 40px;
	}

	.brain-pattern {
		position: relative;
		width: 100%;
		height: 100%;
	}

	.neural-dot {
		position: absolute;
		width: 4px;
		height: 4px;
		background: rgba(100, 200, 255, 0.8);
		border-radius: 50%;
		box-shadow: 0 0 8px rgba(100, 200, 255, 0.6);
		animation: neuralPulse 2s ease-in-out infinite;
	}

	.dot-1 { top: 10px; left: 30px; animation-delay: 0s; }
	.dot-2 { top: 20px; left: 60px; animation-delay: 0.3s; }
	.dot-3 { top: 15px; right: 25px; animation-delay: 0.6s; }

	.neural-connection {
		position: absolute;
		height: 1px;
		background: linear-gradient(90deg, transparent, rgba(100, 200, 255, 0.6), transparent);
		animation: connectionFlow 2s ease-in-out infinite;
	}

	.conn-1 {
		top: 12px;
		left: 34px;
		width: 30px;
		transform: rotate(25deg);
		animation-delay: 0.2s;
	}

	.conn-2 {
		top: 18px;
		left: 55px;
		width: 35px;
		transform: rotate(-15deg);
		animation-delay: 0.5s;
	}

	/* Olhos holográficos */
	.eyes {
		position: absolute;
		top: 60px;
		left: 50%;
		transform: translateX(-50%);
		width: 140px;
		height: 40px;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	.eye {
		position: relative;
		width: 35px;
		height: 35px;
	}

	.eye-core {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 30px;
		height: 30px;
		border-radius: 50%;
		background: radial-gradient(circle, rgba(100, 200, 255, 0.3), transparent 70%);
		border: 2px solid rgba(100, 200, 255, 0.6);
	}

	.iris {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 20px;
		height: 20px;
		border-radius: 50%;
		background: radial-gradient(circle, rgba(100, 200, 255, 0.8), rgba(50, 150, 255, 0.4));
		animation: irisGlow 2s ease-in-out infinite alternate;
	}

	.pupil {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 8px;
		height: 8px;
		border-radius: 50%;
		background: rgba(255, 255, 255, 0.9);
		box-shadow: 0 0 10px rgba(255, 255, 255, 0.8);
		animation: pupilPulse 1.5s ease-in-out infinite;
	}

	.eye-glow {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 40px;
		height: 40px;
		border-radius: 50%;
		background: radial-gradient(circle, transparent 60%, rgba(100, 200, 255, 0.2));
		animation: eyeGlowPulse 3s ease-in-out infinite;
	}

	.eye-scan {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 35px;
		height: 35px;
		border: 1px solid rgba(100, 200, 255, 0.4);
		border-radius: 50%;
		animation: eyeScanRotate 4s linear infinite;
	}

	.eye-scan::before {
		content: '';
		position: absolute;
		top: -1px;
		right: 50%;
		width: 2px;
		height: 100%;
		background: rgba(100, 200, 255, 0.8);
		transform-origin: bottom;
		animation: scannerLine 4s linear infinite;
	}

	/* Nariz geométrico */
	.nose {
		position: absolute;
		top: 110px;
		left: 50%;
		transform: translateX(-50%);
		width: 20px;
		height: 30px;
	}

	.nose-line {
		position: absolute;
		background: rgba(100, 200, 255, 0.6);
		animation: noseGlow 2.5s ease-in-out infinite alternate;
	}

	.line-1 {
		top: 0;
		left: 50%;
		transform: translateX(-50%);
		width: 1px;
		height: 20px;
	}

	.line-2 {
		bottom: 5px;
		left: 50%;
		transform: translateX(-50%);
		width: 12px;
		height: 1px;
	}

	/* Boca holográfica */
	.mouth {
		position: absolute;
		top: 160px;
		left: 50%;
		transform: translateX(-50%);
		width: 60px;
		height: 15px;
	}

	.mouth-line {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 40px;
		height: 2px;
		background: linear-gradient(90deg, transparent, rgba(100, 200, 255, 0.8), transparent);
		border-radius: 10px;
		animation: mouthTalk 2s ease-in-out infinite;
	}

	.mouth-glow {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 50px;
		height: 10px;
		background: radial-gradient(ellipse, rgba(100, 200, 255, 0.2), transparent);
		animation: mouthGlowPulse 2s ease-in-out infinite;
	}

	/* Mandíbula */
	.jawline {
		position: absolute;
		bottom: 20px;
		left: 50%;
		transform: translateX(-50%);
		width: 140px;
		height: 30px;
	}

	.jaw-left, .jaw-right {
		position: absolute;
		bottom: 0;
		width: 60px;
		height: 1px;
		background: linear-gradient(90deg, transparent, rgba(100, 200, 255, 0.6), transparent);
		animation: jawlineGlow 3s ease-in-out infinite alternate;
	}

	.jaw-left {
		left: 10px;
		transform: rotate(-15deg);
		animation-delay: 0s;
	}

	.jaw-right {
		right: 10px;
		transform: rotate(15deg);
		animation-delay: 0.5s;
	}

	/* Grade holográfica */
	.hologram-grid {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		opacity: 0.3;
	}

	.grid-line {
		position: absolute;
		background: rgba(100, 200, 255, 0.2);
	}

	.horizontal {
		width: 100%;
		height: 1px;
		left: 0;
		animation: gridFlicker 4s ease-in-out infinite;
	}

	.vertical {
		height: 100%;
		width: 1px;
		top: 0;
		animation: gridFlicker 4s ease-in-out infinite;
	}

	.h-1 { top: 20%; animation-delay: 0s; }
	.h-2 { top: 35%; animation-delay: 0.5s; }
	.h-3 { top: 50%; animation-delay: 1s; }
	.h-4 { top: 65%; animation-delay: 1.5s; }
	.h-5 { top: 80%; animation-delay: 2s; }

	.v-1 { left: 20%; animation-delay: 0.2s; }
	.v-2 { left: 40%; animation-delay: 0.7s; }
	.v-3 { left: 60%; animation-delay: 1.2s; }
	.v-4 { left: 80%; animation-delay: 1.7s; }

	/* Efeitos de interferência */
	.interference {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		pointer-events: none;
	}

	.glitch-line {
		position: absolute;
		width: 100%;
		height: 2px;
		background: rgba(100, 200, 255, 0.8);
		animation: glitchMove 0.1s linear infinite;
		opacity: 0;
	}

	.g-1 {
		top: 30%;
		animation-delay: 0s;
		animation-duration: 0.15s;
	}

	.g-2 {
		top: 60%;
		animation-delay: 2s;
		animation-duration: 0.12s;
	}

	.g-3 {
		top: 80%;
		animation-delay: 4s;
		animation-duration: 0.18s;
	}

	/* Partículas flutuantes */
	.floating-particles {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		pointer-events: none;
	}

	.particle {
		position: absolute;
		width: 3px;
		height: 3px;
		background: rgba(100, 200, 255, 0.8);
		border-radius: 50%;
		box-shadow: 0 0 6px rgba(100, 200, 255, 0.6);
		animation: particleFloat 4s ease-in-out infinite;
	}

	.p-1 { top: 10%; left: 20%; animation-delay: 0s; }
	.p-2 { top: 25%; right: 15%; animation-delay: 0.5s; }
	.p-3 { top: 45%; left: 10%; animation-delay: 1s; }
	.p-4 { top: 65%; right: 25%; animation-delay: 1.5s; }
	.p-5 { top: 80%; left: 30%; animation-delay: 2s; }
	.p-6 { top: 90%; right: 20%; animation-delay: 2.5s; }

	/* Ativação do holograma */
	.jarvis-container.activated .hologram-face {
		animation: hologramActivation 1s ease-out;
	}

	/* Mensagem do JARVIS */
	.message-container {
		text-align: center;
		background: linear-gradient(145deg, rgba(0, 20, 40, 0.9), rgba(0, 40, 80, 0.8));
		border: 2px solid rgba(100, 200, 255, 0.6);
		border-radius: 15px;
		padding: 20px 30px;
		backdrop-filter: blur(10px);
		box-shadow: 0 0 30px rgba(100, 200, 255, 0.3);
		max-width: 500px;
		position: relative;
	}

	.typing-indicator {
		margin-bottom: 15px;
		display: flex;
		justify-content: center;
		gap: 5px;
	}

	.dot {
		width: 8px;
		height: 8px;
		background: rgba(100, 200, 255, 0.8);
		border-radius: 50%;
		animation: typingDot 1.5s ease-in-out infinite;
	}

	.dot-1 { animation-delay: 0s; }
	.dot-2 { animation-delay: 0.3s; }
	.dot-3 { animation-delay: 0.6s; }

	.message-text {
		font-size: 1.25rem;
		color: rgba(100, 200, 255, 0.95);
		font-weight: 500;
		margin: 0 0 10px 0;
		text-shadow: 0 0 10px rgba(100, 200, 255, 0.5);
		animation: textGlow 3s ease-in-out infinite alternate;
	}

	.message-signature {
		font-size: 0.9rem;
		color: rgba(100, 200, 255, 0.7);
		font-style: italic;
		margin: 0;
	}

	/* Animações do Holograma */
	@keyframes outlineGlow {
		0% { 
			border-color: rgba(100, 200, 255, 0.4);
			box-shadow: 0 0 20px rgba(100, 200, 255, 0.3);
		}
		100% { 
			border-color: rgba(100, 200, 255, 0.8);
			box-shadow: 0 0 40px rgba(100, 200, 255, 0.6);
		}
	}

	@keyframes scanMove {
		0% { 
			top: 0;
			opacity: 0;
		}
		50% { 
			opacity: 1;
		}
		100% { 
			top: 100%;
			opacity: 0;
		}
	}

	@keyframes neuralPulse {
		0%, 100% { 
			box-shadow: 0 0 8px rgba(100, 200, 255, 0.6);
			transform: scale(1);
		}
		50% { 
			box-shadow: 0 0 15px rgba(100, 200, 255, 1);
			transform: scale(1.3);
		}
	}

	@keyframes connectionFlow {
		0% { 
			opacity: 0;
			transform: scaleX(0);
		}
		50% { 
			opacity: 1;
			transform: scaleX(1);
		}
		100% { 
			opacity: 0;
			transform: scaleX(0);
		}
	}

	@keyframes irisGlow {
		0% { 
			background: radial-gradient(circle, rgba(100, 200, 255, 0.8), rgba(50, 150, 255, 0.4));
		}
		100% { 
			background: radial-gradient(circle, rgba(150, 220, 255, 1), rgba(100, 180, 255, 0.8));
		}
	}

	@keyframes pupilPulse {
		0%, 100% { 
			transform: translate(-50%, -50%) scale(1);
			box-shadow: 0 0 10px rgba(255, 255, 255, 0.8);
		}
		50% { 
			transform: translate(-50%, -50%) scale(1.2);
			box-shadow: 0 0 20px rgba(255, 255, 255, 1);
		}
	}

	@keyframes eyeGlowPulse {
		0%, 100% { 
			background: radial-gradient(circle, transparent 60%, rgba(100, 200, 255, 0.2));
		}
		50% { 
			background: radial-gradient(circle, transparent 50%, rgba(100, 200, 255, 0.4));
		}
	}

	@keyframes eyeScanRotate {
		0% { transform: translate(-50%, -50%) rotate(0deg); }
		100% { transform: translate(-50%, -50%) rotate(360deg); }
	}

	@keyframes scannerLine {
		0% { transform: rotate(0deg); }
		100% { transform: rotate(360deg); }
	}

	@keyframes noseGlow {
		0% { 
			background: rgba(100, 200, 255, 0.6);
			box-shadow: 0 0 5px rgba(100, 200, 255, 0.4);
		}
		100% { 
			background: rgba(100, 200, 255, 1);
			box-shadow: 0 0 10px rgba(100, 200, 255, 0.8);
		}
	}

	@keyframes mouthTalk {
		0%, 100% { 
			width: 40px;
			opacity: 0.8;
		}
		25% { 
			width: 30px;
			opacity: 1;
		}
		75% { 
			width: 50px;
			opacity: 0.9;
		}
	}

	@keyframes mouthGlowPulse {
		0%, 100% { 
			background: radial-gradient(ellipse, rgba(100, 200, 255, 0.2), transparent);
		}
		50% { 
			background: radial-gradient(ellipse, rgba(100, 200, 255, 0.4), transparent);
		}
	}

	@keyframes jawlineGlow {
		0% { 
			background: linear-gradient(90deg, transparent, rgba(100, 200, 255, 0.6), transparent);
			box-shadow: 0 0 5px rgba(100, 200, 255, 0.3);
		}
		100% { 
			background: linear-gradient(90deg, transparent, rgba(100, 200, 255, 1), transparent);
			box-shadow: 0 0 10px rgba(100, 200, 255, 0.6);
		}
	}

	@keyframes gridFlicker {
		0%, 90%, 100% { opacity: 0.2; }
		5%, 85% { opacity: 0.6; }
		10%, 80% { opacity: 0.1; }
		15%, 75% { opacity: 0.8; }
	}

	@keyframes glitchMove {
		0% { 
			opacity: 0;
			transform: translateX(-100%);
		}
		20% { 
			opacity: 1;
			transform: translateX(0);
		}
		80% { 
			opacity: 1;
			transform: translateX(0);
		}
		100% { 
			opacity: 0;
			transform: translateX(100%);
		}
	}

	@keyframes particleFloat {
		0%, 100% { 
			transform: translateY(0px) scale(1);
			opacity: 0.6;
		}
		25% { 
			transform: translateY(-15px) scale(1.2);
			opacity: 1;
		}
		75% { 
			transform: translateY(-8px) scale(0.8);
			opacity: 0.8;
		}
	}

	@keyframes hologramActivation {
		0% {
			filter: drop-shadow(0 0 30px rgba(100, 200, 255, 0.6)) brightness(1);
			transform: scale(1);
		}
		30% {
			filter: drop-shadow(0 0 60px rgba(100, 200, 255, 1)) brightness(1.3);
			transform: scale(1.05);
		}
		60% {
			filter: drop-shadow(0 0 80px rgba(100, 200, 255, 1.2)) brightness(1.5);
			transform: scale(1.1);
		}
		100% {
			filter: drop-shadow(0 0 30px rgba(100, 200, 255, 0.6)) brightness(1);
			transform: scale(1);
		}
	}

	@keyframes typingDot {
		0%, 60%, 100% {
			transform: translateY(0);
			opacity: 0.4;
		}
		30% {
			transform: translateY(-10px);
			opacity: 1;
		}
	}

	@keyframes textGlow {
		0% { text-shadow: 0 0 10px rgba(100, 200, 255, 0.5); }
		100% { text-shadow: 0 0 20px rgba(100, 200, 255, 0.8); }
	}
</style>