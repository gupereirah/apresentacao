<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-3xl font-bold text-white mb-3 drop-shadow-lg">
		🛠️ Kit de Sobrevivência
	</h1>
	<p class="text-base text-white/90 leading-relaxed drop-shadow mb-4">
		Ferramentas, plataformas e comunidades essenciais 🚀
	</p>
	
	<div class="max-w-6xl mx-auto space-y-3">
		<!-- Onde Estudar e Ferramentas & Comunidades -->
		<div class="grid grid-cols-2 gap-3">
			<!-- Plataformas de Estudo -->
			<div class="bg-gradient-to-r from-blue-500/20 to-purple-500/20 backdrop-blur-sm rounded-xl p-3 border border-blue-300/30">
				<h3 class="text-lg font-bold text-white mb-2 flex items-center justify-center">
					📚 <span class="ml-2">Onde Estudar</span>
				</h3>
				<div class="grid grid-cols-2 gap-2">
					<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 text-center">
						<div class="text-sm mb-1">📺</div>
						<h4 class="text-xs font-bold text-white">YouTube</h4>
						<p class="text-white/70 text-xs">Gratuito</p>
					</div>
					<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 text-center">
						<div class="text-sm mb-1">🎓</div>
						<h4 class="text-xs font-bold text-white">Alura</h4>
						<p class="text-white/70 text-xs">Brasileiro</p>
					</div>
					<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 text-center">
						<div class="text-sm mb-1">💻</div>
						<h4 class="text-xs font-bold text-white">FreeCodeCamp</h4>
						<p class="text-white/70 text-xs">Certificados</p>
					</div>
					<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 text-center">
						<div class="text-sm mb-1">🚀</div>
						<h4 class="text-xs font-bold text-white">Udemy</h4>
						<p class="text-white/70 text-xs">Prático</p>
					</div>
				</div>
			</div>
			
			<!-- Ferramentas e Comunidades -->
			<div class="bg-gradient-to-r from-green-500/20 to-emerald-500/20 backdrop-blur-sm rounded-xl p-3 border border-green-300/30">
				<h3 class="text-lg font-bold text-white mb-2 text-center">
					🔧 Ferramentas & Comunidades
				</h3>
				<div class="grid grid-cols-2 gap-2">
					<div class="space-y-2">
						<h4 class="text-sm font-bold text-white text-center mb-1">Ferramentas</h4>
						<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 flex items-center">
							<span class="text-sm mr-2">🐙</span>
							<div class="text-left">
								<h4 class="text-xs font-bold text-white">GitHub</h4>
								<p class="text-white/70 text-xs">Portfólio</p>
							</div>
						</div>
						<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 flex items-center">
							<span class="text-sm mr-2">🤖</span>
							<div class="text-left">
								<h4 class="text-xs font-bold text-white">Cursor</h4>
								<p class="text-white/70 text-xs">Editor IA</p>
							</div>
						</div>
					</div>
					<div class="space-y-2">
						<h4 class="text-sm font-bold text-white text-center mb-1">Comunidades</h4>
						<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 flex items-center">
							<span class="text-sm mr-2">💼</span>
							<div class="text-left">
								<h4 class="text-xs font-bold text-white">LinkedIn</h4>
								<p class="text-white/70 text-xs">Networking</p>
							</div>
						</div>
						<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 border border-white/20 flex items-center">
							<span class="text-sm mr-2">❓</span>
							<div class="text-left">
								<h4 class="text-xs font-bold text-white">Stack Overflow</h4>
								<p class="text-white/70 text-xs">Dúvidas</p>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
		
		<!-- Ferramentas de IA para Devs -->
		<div class="bg-gradient-to-r from-purple-500/20 to-indigo-500/20 backdrop-blur-sm rounded-xl p-4 border border-purple-300/30">
			<h3 class="text-xl font-bold text-white mb-3 text-center">
				🤖 Era da IA para Devs
			</h3>
			<div class="grid grid-cols-4 gap-3">
				<div class="bg-white/10 backdrop-blur-sm rounded-lg p-3 border border-white/20 text-center">
					<div class="text-lg mb-2">🧠</div>
					<h4 class="text-sm font-bold text-white">ChatGPT</h4>
					<p class="text-white/70 text-xs">Explicações e debug</p>
				</div>
				<div class="bg-white/10 backdrop-blur-sm rounded-lg p-3 border border-white/20 text-center">
					<div class="text-lg mb-2">🚀</div>
					<h4 class="text-sm font-bold text-white">GitHub Copilot</h4>
					<p class="text-white/70 text-xs">Autocompletar código</p>
				</div>
				<div class="bg-gradient-to-r from-blue-500/30 to-purple-500/30 backdrop-blur-sm rounded-lg p-3 border border-blue-400/50 text-center">
					<div class="text-lg mb-2">⚡</div>
					<h4 class="text-sm font-bold text-white">Claude/Cursor</h4>
					<p class="text-white/90 text-xs font-semibold">Pair programming</p>
				</div>
				<div class="bg-white/10 backdrop-blur-sm rounded-lg p-3 border border-white/20 text-center">
					<div class="text-lg mb-2">💎</div>
					<h4 class="text-sm font-bold text-white">Gemini</h4>
					<p class="text-white/70 text-xs">Código e queries</p>
				</div>
			</div>
			<div class="mt-4 bg-white/5 backdrop-blur-sm rounded-lg p-3 border border-white/10">
				<p class="text-white/90 text-sm text-center">
					🚀 <strong>O futuro chegou:</strong> IA acelera desenvolvimento e potencializa criatividade!
				</p>
			</div>
			<div class="mt-3 bg-gradient-to-r from-yellow-500/20 to-orange-500/20 backdrop-blur-sm rounded-lg p-3 border border-yellow-300/30">
				<p class="text-white font-bold text-sm text-center">
					⚡ <strong>IA não substitui devs, mas devs que usam IA substituem os que não usam!</strong>
				</p>
			</div>
		</div>
	</div>
</div>

<style>
	.slide-content {
		@apply text-center;
	}
</style>