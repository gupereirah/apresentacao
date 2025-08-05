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
			
			<div class="space-y-12">
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
							<h3 class="text-2xl font-bold text-white mb-3">🔍 Analista de Qualidade</h3>
							<ul class="text-lg text-white/80 text-left space-y-1">
								<li>• Testes manuais</li>
								<li>• Quebrava sistemas</li>
								<li>• Validava entregas técnicas</li>
							</ul>
						</div>
					</div>
				</div>
			</div>
		</div>
		
		<div class="mt-12 text-center">
			<p class="text-lg text-white/70">
				🎯 <strong>Momento chave:</strong> Cada função me aproximava mais do desenvolvimento
			</p>
		</div>
	</div>
</div>

<style>
	.slide-content {
		@apply text-center;
	}
</style>