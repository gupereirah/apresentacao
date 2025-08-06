<script>
	export const isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-6 md:mb-6 drop-shadow-lg px-4">
		📈 Crescimento Interno
	</h1>
	<p class="text-xl md:text-2xl lg:text-3xl text-white/90 leading-relaxed drop-shadow mb-8 md:mb-5 px-4">
		Evoluindo dentro da empresa
	</p>
	
		<div class="w-full max-w-full mx-auto px-4">
		<!-- Blocos separados -->
		<div class="space-y-12 lg:space-y-6">
			<!-- Analista de Produto -->
			<div class="w-full">
				<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-6 md:p-8 lg:p-10 border border-white/20 w-full">
					<h3 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white mb-4 md:mb-6 text-center">📋 Analista de Produto e Desenvolvimento</h3>
					<p class="text-xl md:text-2xl lg:text-3xl text-white/80 leading-relaxed text-center">Evolução natural das responsabilidades</p>
				</div>
			</div>
			
			<!-- Analista de Qualidade -->
			<div class="w-full">
				<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-6 md:p-8 lg:p-10 border border-white/20 w-full">
					<h3 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white mb-4 md:mb-6 text-center">🔍 Analista de Qualidade</h3>
					<div class="text-left space-y-4 md:space-y-6">
						<div class="flex items-start space-x-4">
							<span class="text-green-400 text-2xl md:text-3xl flex-shrink-0">🧪</span>
							<div>
								<p class="text-xl md:text-2xl lg:text-3xl font-semibold text-white mb-2">Testes manuais</p>
								<p class="text-lg md:text-xl lg:text-2xl text-white/70 leading-relaxed">Execução de cenários de teste e validação de funcionalidades</p>
							</div>
						</div>
						<div class="flex items-start space-x-4">
							<span class="text-orange-400 text-2xl md:text-3xl flex-shrink-0">🔍</span>
							<div>
								<p class="text-xl md:text-2xl lg:text-3xl font-semibold text-white mb-2">Testes exploratórios</p>
								<p class="text-lg md:text-xl lg:text-2xl text-white/70 leading-relaxed">Identificação proativa de falhas e vulnerabilidades do sistema</p>
							</div>
						</div>
						<div class="flex items-start space-x-4">
							<span class="text-blue-400 text-2xl md:text-3xl flex-shrink-0">✅</span>
							<div>
								<p class="text-xl md:text-2xl lg:text-3xl font-semibold text-white mb-2">Validava entregas técnicas</p>
								<p class="text-lg md:text-xl lg:text-2xl text-white/70 leading-relaxed">Garantia de qualidade e conformidade com os requisitos</p>
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