<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-6xl font-bold text-white mb-8 drop-shadow-lg">
		📈 Crescimento Interno
	</h1>
	<p class="text-2xl text-white/90 leading-relaxed drop-shadow mb-12">
		Evoluindo dentro da empresa
	</p>
	
	<div class="max-w-6xl mx-auto">
		<!-- Timeline de evolução -->
		<div class="relative">
			<div class="absolute left-1/2 transform -translate-x-1/2 h-full w-1 bg-gradient-to-b from-blue-400 to-purple-400 rounded-full"></div>
			
			<div class="space-y-1">
				<!-- Analista de Produto -->
				<div class="flex items-center">
					<div class="w-1/2 pr-8 text-right">
						<div class="bg-white/10 backdrop-blur-sm rounded-2xl p-6 border border-white/20">
							<h3 class="text-2xl font-bold text-white mb-3">📋 Analista de Produto e Desenvolvimento</h3>
							<p class="text-lg text-white/80">Evolução natural das responsabilidades</p>
						</div>
					</div>
					<div class="w-6 h-6 bg-blue-400 rounded-full border-4 border-white z-10"></div>
					<div class="w-1/2 pl-8"></div>
				</div>
				
				<!-- Analista de Qualidade -->
				<div class="flex items-center">
					<div class="w-1/2 pr-8"></div>
					<div class="w-6 h-6 bg-purple-400 rounded-full border-4 border-white z-10"></div>
					<div class="w-1/2 pl-8">
						<div class="bg-white/10 backdrop-blur-sm rounded-2xl p-6 border border-white/20">
							<h3 class="text-2xl font-bold text-white mb-4">🔍 Analista de Qualidade</h3>
							<div class="text-left space-y-3">
								<div class="flex items-start space-x-3">
									<span class="text-green-400 text-xl">🧪</span>
									<div>
										<p class="text-lg font-semibold text-white">Testes manuais</p>
										<p class="text-sm text-white/70">Execução de cenários de teste e validação de funcionalidades</p>
									</div>
								</div>
								<div class="flex items-start space-x-3">
									<span class="text-orange-400 text-xl">🔍</span>
									<div>
										<p class="text-lg font-semibold text-white">Testes exploratórios</p>
										<p class="text-sm text-white/70">Identificação proativa de falhas e vulnerabilidades do sistema</p>
									</div>
								</div>
								<div class="flex items-start space-x-3">
									<span class="text-blue-400 text-xl">✅</span>
									<div>
										<p class="text-lg font-semibold text-white">Validava entregas técnicas</p>
										<p class="text-sm text-white/70">Garantia de qualidade e conformidade com os requisitos</p>
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
		@apply text-center;
	}
</style>