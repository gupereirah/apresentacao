<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-6xl font-bold text-white mb-8 drop-shadow-lg">
		🎉 Obrigado!
	</h1>
	<p class="text-2xl text-white/90 leading-relaxed drop-shadow mb-12">
		Espero ter inspirado vocês com minha jornada
	</p>
	
	<!-- Slide final com elementos especiais -->
	<div class="max-w-5xl mx-auto space-y-8">
		<div class="bg-gradient-to-r from-blue-500/20 to-purple-500/20 backdrop-blur-sm rounded-3xl p-12 border border-blue-300/30">
			<h3 class="text-4xl font-bold text-white mb-8">✨ Resumo da Jornada</h3>
			<div class="grid grid-cols-3 gap-8 text-center">
				<div>
					<div class="text-4xl mb-4">🏢</div>
					<p class="text-white/90 font-semibold">Suporte Técnico</p>
					<p class="text-white/70 text-sm">HP - Base técnica</p>
				</div>
				<div>
					<div class="text-4xl mb-4">🔍</div>
					<p class="text-white/90 font-semibold">Analista de QA</p>
					<p class="text-white/70 text-sm">Automação de testes</p>
				</div>
				<div>
					<div class="text-4xl mb-4">👨‍💻</div>
					<p class="text-white/90 font-semibold">Dev Sênior</p>
					<p class="text-white/70 text-sm">Febrafar - Realização</p>
				</div>
			</div>
		</div>
		
		<!-- Contato -->
		<div class="bg-gradient-to-r from-green-500/20 to-emerald-500/20 backdrop-blur-sm rounded-3xl p-8 border border-green-300/30">
			<h3 class="text-2xl font-bold text-white mb-4">📧 Vamos conversar?</h3>
			<p class="text-lg text-white/90">
				Estou sempre disponível para ajudar quem está começando na área!
			</p>
		</div>
		
		<div class="text-lg text-white/70">
			<p>Pressione <kbd class="bg-white/20 px-2 py-1 rounded text-sm">Home</kbd> para voltar ao início</p>
		</div>
	</div>
</div>

<style>
	.slide-content {
		@apply text-center;
	}
</style>