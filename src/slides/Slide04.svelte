<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold text-white mb-6 md:mb-8 drop-shadow-lg px-4">
		📈 Crescimento Interno
	</h1>
	<p class="text-xl md:text-2xl lg:text-3xl text-white/90 leading-relaxed drop-shadow mb-8 md:mb-12 px-4">
		Evoluindo dentro da empresa
	</p>
	
	<div class="max-w-xs sm:max-w-4xl md:max-w-5xl lg:max-w-6xl mx-auto px-4">
		<!-- Timeline de evolução -->
		<div class="relative">
			<div class="absolute left-1/2 transform -translate-x-1/2 h-full w-1 bg-gradient-to-b from-blue-400 to-purple-400 rounded-full hidden lg:block"></div>
			
			<div class="space-y-6 lg:space-y-1">
				<!-- Analista de Produto -->
				<div class="flex flex-col lg:flex-row items-center">
					<div class="w-full lg:w-1/2 lg:pr-8 text-center lg:text-right mb-4 lg:mb-0">
						<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-4 md:p-6 border border-white/20">
							<h3 class="text-xl md:text-2xl lg:text-3xl font-bold text-white mb-2 md:mb-3">📋 Analista de Produto e Desenvolvimento</h3>
							<p class="text-lg md:text-xl text-white/80">Evolução natural das responsabilidades</p>
						</div>
					</div>
					<div class="w-6 h-6 bg-blue-400 rounded-full border-4 border-white z-10 hidden lg:block"></div>
					<div class="w-full lg:w-1/2 lg:pl-8"></div>
				</div>
				
				<!-- Analista de Qualidade -->
				<div class="flex flex-col lg:flex-row items-center">
					<div class="w-full lg:w-1/2 lg:pr-8 order-2 lg:order-1"></div>
					<div class="w-6 h-6 bg-purple-400 rounded-full border-4 border-white z-10 hidden lg:block order-1 lg:order-2"></div>
					<div class="w-full lg:w-1/2 lg:pl-8 order-1 lg:order-3">
						<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-4 md:p-6 border border-white/20">
							<h3 class="text-xl md:text-2xl lg:text-3xl font-bold text-white mb-3 md:mb-4 text-center lg:text-left">🔍 Analista de Qualidade</h3>
							<div class="text-left space-y-3">
								<div class="flex items-start space-x-3">
									<span class="text-green-400 text-lg md:text-xl">🧪</span>
									<div>
										<p class="text-lg md:text-xl font-semibold text-white">Testes manuais</p>
										<p class="text-sm md:text-base text-white/70">Execução de cenários de teste e validação de funcionalidades</p>
									</div>
								</div>
								<div class="flex items-start space-x-3">
									<span class="text-orange-400 text-lg md:text-xl">🔍</span>
									<div>
										<p class="text-lg md:text-xl font-semibold text-white">Testes exploratórios</p>
										<p class="text-sm md:text-base text-white/70">Identificação proativa de falhas e vulnerabilidades do sistema</p>
									</div>
								</div>
								<div class="flex items-start space-x-3">
									<span class="text-blue-400 text-lg md:text-xl">✅</span>
									<div>
										<p class="text-lg md:text-xl font-semibold text-white">Validava entregas técnicas</p>
										<p class="text-sm md:text-base text-white/70">Garantia de qualidade e conformidade com os requisitos</p>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
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
			font-size: 1.25rem; /* text-xl */
		}
		.slide-content p {
			font-size: 1rem; /* text-base */
		}
	}
</style>