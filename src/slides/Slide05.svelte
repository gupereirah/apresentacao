<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold text-white mb-6 md:mb-8 drop-shadow-lg px-4">
		🎯 Primeiro Grande Desafio
	</h1>

	<div class="max-w-xs sm:max-w-4xl md:max-w-5xl lg:max-w-6xl mx-auto space-y-6 md:space-y-8 px-4">
		<!-- Desafio proposto -->
		<div class="bg-gradient-to-r from-red-500/20 to-orange-500/20 backdrop-blur-sm rounded-2xl md:rounded-3xl p-6 md:p-8 lg:p-10 border border-red-300/30">
			<h3 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white mb-4 md:mb-6 flex flex-col sm:flex-row items-center justify-center">
				⚡ <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">Desafio Proposto</span>
			</h3>
			<p class="text-xl md:text-2xl lg:text-3xl text-white/90 text-center mb-6 md:mb-8">
				"Automatizar testes na empresa"
			</p>
			
			<div class="grid grid-cols-1 lg:grid-cols-2 gap-6 md:gap-8">
				<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-4 md:p-6 border border-white/20">
					<h4 class="text-xl md:text-2xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center">
						📚 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Curso QA Academy</span>
					</h4>
					<ul class="text-lg md:text-xl text-white/90 space-y-2 text-left">
						<li>• Java</li>
						<li>• Selenium</li>
						<li>• Gherkin</li>
					</ul>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-4 md:p-6 border border-white/20">
					<h4 class="text-xl md:text-2xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center">
						😰 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Primeira Dificuldade</span>
					</h4>
					<p class="text-lg md:text-xl text-white/90 text-left">
						<strong>Lógica de programação</strong><br>
						<span class="text-base md:text-lg text-white/70">Não entendia como as coisas funcionavam de fato aplicadas</span>
					</p>
				</div>
			</div>
		</div>
		
		<div class="text-center">
			<div class="inline-block bg-green-500/20 backdrop-blur-sm rounded-xl lg:rounded-2xl px-6 md:px-8 py-3 md:py-4 border border-green-300/30">
				<p class="text-xl md:text-2xl text-white font-semibold">
					✅ <strong>Resultado:</strong> Consegui desenvolver automações!
				</p>
			</div>
		</div>
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
		.slide-content h3 {
			font-size: 1.5rem; /* text-2xl */
		}
		.slide-content p {
			font-size: 1rem; /* text-base */
		}
	}
</style>