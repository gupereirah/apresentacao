<script>
	import { onMount } from 'svelte';
	
		// Importar slides essenciais (otimizado para 30 minutos)
	import Slide01 from '../slides/Slide01.svelte';
	import Slide02 from '../slides/Slide02.svelte';
	import Slide03 from '../slides/Slide03.svelte';
	import Slide04 from '../slides/Slide04.svelte';
	import Slide05 from '../slides/Slide05.svelte';
	import Slide06 from '../slides/Slide06.svelte';
	import Slide07 from '../slides/Slide07.svelte';
	import Slide08 from '../slides/Slide08.svelte';
	import Slide09 from '../slides/Slide09.svelte';
	import Slide10 from '../slides/Slide10.svelte';

	import Slide11 from '../slides/Slide11.svelte';
	import Slide12 from '../slides/Slide12.svelte';
	import Slide13 from '../slides/Slide13.svelte';

	let currentStep = 1;
	const totalSteps = 13;

	// Array com os componentes dos slides (13 slides essenciais)
	const slideComponents = [
		Slide01, Slide02, Slide03, Slide04, Slide05,
		Slide06, Slide07, Slide08, Slide09, Slide10,
		Slide11, Slide12, Slide13
	];
	
	// Função para avançar slide
	function nextSlide() {
		if (currentStep < totalSteps) {
			currentStep++;
		}
	}
	
	// Função para voltar slide
	function prevSlide() {
		if (currentStep > 1) {
			currentStep--;
		}
	}
	
	// Função para ir para um slide específico
	function goToSlide(step) {
		if (step >= 1 && step <= totalSteps) {
			currentStep = step;
		}
	}
	
	// Event listener para teclado
	function handleKeydown(event) {
		switch (event.key) {
			case 'ArrowRight':
			case 'Enter':
			case ' ': // Espaço
				event.preventDefault();
				nextSlide();
				break;
			case 'ArrowLeft':
				event.preventDefault();
				prevSlide();
				break;
			case 'Home':
				event.preventDefault();
				goToSlide(1);
				break;
			case 'End':
				event.preventDefault();
				goToSlide(totalSteps);
				break;
		}
	}
	
	onMount(() => {
		// Adicionar event listener para teclado
		document.addEventListener('keydown', handleKeydown);
		
		// Cleanup
		return () => {
			document.removeEventListener('keydown', handleKeydown);
		};
	});
</script>

<!-- Apresentação em fullscreen -->
<div class="min-h-screen bg-gradient-to-br from-teal-700 via-blue-800 to-green-700 flex items-center justify-center relative overflow-hidden">
	
	<!-- Slide atual -->
	<div class="w-full max-w-6xl mx-auto px-8 h-full flex items-center">
		<div class="{currentStep === 13 ? 'bg-white/5 backdrop-blur-xl shadow-sm' : 'bg-white/10 backdrop-blur-lg p-8 border border-white/20 shadow-2xl'} rounded-3xl w-full max-h-[80vh] overflow-y-auto">
			<!-- Renderizar o componente do slide atual -->
			<svelte:component this={slideComponents[currentStep - 1]} isActive={true} />
		</div>
	</div>
	
	<!-- Navegação com setas -->
	<div class="absolute left-8 top-1/2 transform -translate-y-1/2">
		<button 
			on:click={prevSlide}
			disabled={currentStep === 1}
			aria-label="Slide anterior"
			class="bg-white/20 hover:bg-white/30 disabled:opacity-50 disabled:cursor-not-allowed backdrop-blur-sm rounded-full p-4 transition-all duration-200 border border-white/20 hover:scale-110"
		>
			<svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
				<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"></path>
			</svg>
		</button>
	</div>
	
	<div class="absolute right-8 top-1/2 transform -translate-y-1/2">
		<button 
			on:click={nextSlide}
			disabled={currentStep === totalSteps}
			aria-label="Próximo slide"
			class="bg-white/20 hover:bg-white/30 disabled:opacity-50 disabled:cursor-not-allowed backdrop-blur-sm rounded-full p-4 transition-all duration-200 border border-white/20 hover:scale-110"
		>
			<svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
				<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path>
			</svg>
		</button>
	</div>
	
	<!-- Indicador de progresso -->
	<div class="absolute bottom-8 left-1/2 transform -translate-x-1/2">
		<div class="flex items-center space-x-2 bg-white/10 backdrop-blur-sm rounded-full px-6 py-2 border border-white/20">
			<div class="text-white text-sm font-medium">
				{currentStep} / {totalSteps}
			</div>
			<div class="w-32 h-2 bg-white/20 rounded-full overflow-hidden">
				<div 
					class="h-full bg-gradient-to-r from-teal-400 to-blue-400 rounded-full progress-bar"
					style="width: {(currentStep / totalSteps) * 100}%"
				></div>
			</div>
		</div>
	</div>
	
</div>

<style>
	/* Efeito de hover nos botões de navegação */
	button:hover {
		transform: scale(1.1);
		backdrop-filter: blur(10px);
	}
	
	button:active {
		transform: scale(1.05);
	}
	
	/* Transição suave dos botões */
	button {
		transition: all 0.2s ease;
	}
	
	/* Animação suave para o indicador de progresso */
	.progress-bar {
		transition: width 0.3s ease;
	}
</style>
