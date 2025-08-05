<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-4xl font-bold text-white mb-4 drop-shadow-lg">
		📈 Linha do Tempo Resumida
	</h1>
	<p class="text-lg text-white/90 leading-relaxed drop-shadow mb-6">
		Minha jornada em etapas principais
	</p>
	
	<div class="max-w-5xl mx-auto">
		<div class="relative">
			<!-- Linha do tempo vertical -->
			<div class="absolute left-1/2 transform -translate-x-1/2 h-full w-1 bg-gradient-to-b from-blue-400 via-purple-400 to-green-400 rounded-full"></div>
			
			<div class="space-y-6">
				<!-- HP -->
				<div class="flex items-center">
					<div class="w-1/2 text-right pr-8">
						<div class="bg-gradient-to-r from-blue-500/20 to-cyan-500/20 backdrop-blur-sm rounded-xl p-4 border border-blue-300/30">
							<h4 class="text-lg font-bold text-white mb-1">🏢 HP (2011-2013)</h4>
							<p class="text-white/80 text-sm">Suporte técnico → "O cara da impressora"</p>
						</div>
					</div>
					<div class="w-4 h-4 bg-blue-400 rounded-full border-4 border-white z-10"></div>
					<div class="w-1/2"></div>
				</div>
				
				<!-- Febrafar Início -->
				<div class="flex items-center">
					<div class="w-1/2"></div>
					<div class="w-4 h-4 bg-purple-400 rounded-full border-4 border-white z-10"></div>
					<div class="w-1/2 text-left pl-8">
						<div class="bg-gradient-to-r from-purple-500/20 to-pink-500/20 backdrop-blur-sm rounded-xl p-4 border border-purple-300/30">
							<h4 class="text-lg font-bold text-white mb-1">🏥 Febrafar (2013-2017)</h4>
							<p class="text-white/80 text-sm">Assistente → Analista → QA</p>
						</div>
					</div>
				</div>
				
				<!-- Virada Dev -->
				<div class="flex items-center">
					<div class="w-1/2 text-right pr-8">
						<div class="bg-gradient-to-r from-green-500/20 to-emerald-500/20 backdrop-blur-sm rounded-xl p-4 border border-green-300/30">
							<h4 class="text-lg font-bold text-white mb-1">🚀 Virada Dev (2017-2020)</h4>
							<p class="text-white/80 text-sm">QA → Dev Jr → Pleno</p>
						</div>
					</div>
					<div class="w-4 h-4 bg-green-400 rounded-full border-4 border-white z-10"></div>
					<div class="w-1/2"></div>
				</div>
				
				<!-- Dev Sênior -->
				<div class="flex items-center">
					<div class="w-1/2"></div>
					<div class="w-4 h-4 bg-yellow-400 rounded-full border-4 border-white z-10"></div>
					<div class="w-1/2 text-left pl-8">
						<div class="bg-gradient-to-r from-yellow-500/20 to-orange-500/20 backdrop-blur-sm rounded-xl p-4 border border-yellow-300/30">
							<h4 class="text-lg font-bold text-white mb-1">⭐ Dev Sênior (2020-hoje)</h4>
							<p class="text-white/80 text-sm">Liderança técnica e mentoria</p>
						</div>
					</div>
				</div>
			</div>
		</div>
		
		<!-- Resumo -->
		<div class="mt-8 bg-gradient-to-r from-white/10 to-white/5 backdrop-blur-sm rounded-2xl p-6 border border-white/20">
			<h3 class="text-xl font-bold text-white mb-3">🎯 Resumo da Jornada</h3>
			<p class="text-white/90">
				<strong>9+ anos</strong> de evolução constante: do suporte técnico ao desenvolvimento sênior.
				<br>A chave foi <strong>aproveitar oportunidades internas</strong> e <strong>nunca parar de aprender</strong>! 🚀
			</p>
		</div>
	</div>
</div>

<style>
	.slide-content {
		@apply text-center;
	}
</style>