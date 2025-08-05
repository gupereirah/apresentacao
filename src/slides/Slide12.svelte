<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-4xl font-bold text-white mb-4 drop-shadow-lg">
		🛠️ Kit de Sobrevivência - Parte 1
	</h1>
	<p class="text-lg text-white/90 leading-relaxed drop-shadow mb-6">
		Plataformas para estudar sem quebrar o cofrinho 💰
	</p>
	
	<div class="max-w-6xl mx-auto space-y-4">
		<!-- Plataformas Gratuitas -->
		<div class="bg-gradient-to-r from-green-500/20 to-emerald-500/20 backdrop-blur-sm rounded-2xl p-6 border border-green-300/30">
			<h3 class="text-2xl font-bold text-white mb-4 flex items-center justify-center">
				🆓 <span class="ml-3">Gratuitas (o melhor preço!)</span>
			</h3>
			<div class="grid grid-cols-2 gap-4">
				<div class="bg-white/10 backdrop-blur-sm rounded-xl p-4 border border-white/20 text-center">
					<div class="text-3xl mb-3">📺</div>
					<h4 class="text-lg font-bold text-white mb-2">YouTube</h4>
					<p class="text-white/80 text-sm">Curso em Vídeo, Rocketseat, Code/Drops</p>
				</div>
				<div class="bg-white/10 backdrop-blur-sm rounded-xl p-4 border border-white/20 text-center">
					<div class="text-3xl mb-3">💻</div>
					<h4 class="text-lg font-bold text-white mb-2">FreeCodeCamp</h4>
					<p class="text-white/80 text-sm">Certificações práticas e gratuitas</p>
				</div>
			</div>
		</div>

		<!-- Plataformas Pagas (mas que valem a pena) -->
		<div class="bg-gradient-to-r from-blue-500/20 to-purple-500/20 backdrop-blur-sm rounded-2xl p-6 border border-blue-300/30">
			<h3 class="text-2xl font-bold text-white mb-4 flex items-center justify-center">
				💎 <span class="ml-3">Pagas (investimento que vale a pena)</span>
			</h3>
			<div class="grid grid-cols-3 gap-4">
				<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 text-center">
					<div class="text-xl mb-1">🎓</div>
					<h4 class="text-xs font-bold text-white">Alura</h4>
					<p class="text-white/80 text-xs">Brasileira</p>
				</div>
				<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 text-center">
					<div class="text-xl mb-1">🏫</div>
					<h4 class="text-xs font-bold text-white">Coursera</h4>
					<p class="text-white/80 text-xs">Universidades</p>
				</div>
				<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 text-center">
					<div class="text-xl mb-1">🚀</div>
					<h4 class="text-xs font-bold text-white">Udemy</h4>
					<p class="text-white/80 text-xs">Práticos</p>
				</div>
			</div>
		</div>

		<!-- Dica especial -->
		<div class="bg-gradient-to-r from-yellow-500/20 to-orange-500/20 backdrop-blur-sm rounded-2xl p-6 border border-yellow-300/30">
			<h3 class="text-xl font-bold text-white mb-3 flex items-center justify-center">
				💡 <span class="ml-3">Dica de Ouro</span>
			</h3>
			<p class="text-lg text-white/90 text-center">
				Comece pelo <strong>gratuito</strong>, veja se gosta, depois invista no pago. 
				<br>Não precisa fazer 10 cursos ao mesmo tempo! 😅
			</p>
		</div>
	</div>
</div>

<style>
	.slide-content {
		@apply text-center;
	}
</style>