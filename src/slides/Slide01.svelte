<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold text-white mb-6 md:mb-8 drop-shadow-lg px-4">
		Desafios da Carreira de Desenvolvedor
	</h1>
	<p class="text-xl md:text-2xl lg:text-3xl text-white/90 leading-relaxed drop-shadow mb-8 md:mb-12 px-4">
		Um pouco sobre a minha jornada
	</p>
	
	<div class="max-w-xs sm:max-w-2xl md:max-w-3xl lg:max-w-4xl mx-auto px-4">
		<div class="bg-gradient-to-r from-white/20 to-white/10 backdrop-blur-sm rounded-2xl md:rounded-3xl p-6 md:p-8 lg:p-12 border border-white/30">
			<div class="text-4xl md:text-5xl mb-4 md:mb-6">👨‍💻</div>
			<h2 class="text-4xl md:text-5xl font-bold text-white mb-3 md:mb-4">Gustavo</h2>
			<p class="text-2xl md:text-3xl text-white/90 mb-3 md:mb-4">Desenvolvedor Sênior – Febrafar</p>
			<p class="text-xl md:text-2xl text-white/80 leading-relaxed">
				Formado em Ciência da Computação e Sistemas de Informação pela UNIP
			</p>
		</div>
	</div>
	
	<div class="mt-6 md:mt-8 px-4">
		<p class="text-2xl md:text-3xl text-white/70 max-w-4xl mx-auto leading-relaxed">
			<strong>Objetivo:</strong> Abordar obstáculos comuns no início da carreira e estratégias para superá-los
		</p>
	</div>
</div>

<style>
	.slide-content {
		text-align: center;
		min-height: 100vh;
		display: flex;
		flex-direction: column;
		justify-content: center;
		padding: 2rem 0;
	}
	
	/* Ajustes adicionais para telas muito pequenas */
	@media (max-width: 320px) {
		.slide-content h1 {
			font-size: 2.25rem; /* text-4xl */
		}
		.slide-content p {
			font-size: 1rem; /* text-base */
		}
	}
</style>