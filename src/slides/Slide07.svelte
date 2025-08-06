<script>
	export const isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-4 md:mb-4 drop-shadow-lg px-4">
		😰 A Realidade da Transição
	</h1>

	<div class="max-w-xs sm:max-w-4xl md:max-w-5xl lg:max-w-[80%] mx-auto space-y-6 px-4">
		<!-- O choque da realidade -->
		<div class="bg-gradient-to-r from-red-500/20 to-pink-500/20 backdrop-blur-sm rounded-2xl md:rounded-3xl p-4 md:p-6 border border-red-300/30">
			<h3 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-4 md:mb-6 flex flex-col lg:flex-row items-center justify-center">
				⚡ <span class="ml-0 lg:ml-3 mt-2 lg:mt-0 text-center">As dificuldades que ninguém te conta quando você quer virar desenvolvedor</span>
			</h3>
			<div class="grid grid-cols-1 lg:grid-cols-2 gap-4 md:gap-6">
				<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-3 md:p-4 border border-white/20">
					<h4 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center">
						🤯 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Síndrome do Impostor</span>
					</h4>
					<ul class="text-xl md:text-2xl lg:text-3xl text-white/90 space-y-3 md:space-y-4 text-left">
						<li>• "Todo mundo sabe mais que eu"</li>
						<li>• "Vou ser descoberto como fraude"</li>
						<li>• "Não deveria estar aqui"</li>
					</ul>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-3 md:p-4 border border-white/20">
					<h4 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center">
						🌊 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Sobrecarga de Informação</span>
					</h4>
					<ul class="text-xl md:text-2xl lg:text-3xl text-white/90 space-y-3 md:space-y-4 text-left">
						<li>• Frameworks novos toda semana</li>
						<li>• "Preciso aprender TUDO agora"</li>
						<li>• Paralisia por análise</li>
					</ul>
				</div>
			</div>
		</div>
		
		<!-- O que eu gostaria de ter sabido -->
		<div class="bg-gradient-to-r from-blue-500/20 to-cyan-500/20 backdrop-blur-sm rounded-2xl md:rounded-3xl p-4 md:p-6 border border-blue-300/30">
			<div class="grid grid-cols-1 md:grid-cols-3 gap-3 md:gap-4">
				<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-3 md:p-4 border border-white/20 text-center">
					<div class="text-2xl md:text-3xl mb-1 md:mb-2">🎯</div>
					<h4 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-2 md:mb-3">Foque no Básico</h4>
					<p class="text-lg md:text-xl lg:text-2xl text-white/80">Não precisa saber 10 frameworks. Domine os fundamentos primeiro.</p>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-3 md:p-4 border border-white/20 text-center">
					<div class="text-2xl md:text-3xl mb-1 md:mb-2">🤝</div>
					<h4 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-2 md:mb-3">Seja Genuinamente Legal</h4>
					<p class="text-lg md:text-xl lg:text-2xl text-white/80">Ajude outros, participe de comunidades, seja você mesmo. Conexões naturais são mais valiosas.</p>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-3 md:p-4 border border-white/20 text-center">
					<div class="text-2xl md:text-3xl mb-1 md:mb-2">⏰</div>
					<h4 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-2 md:mb-3">Paciência</h4>
					<p class="text-lg md:text-xl lg:text-2xl text-white/80">Crescimento leva tempo. Não compare seu capítulo 1 com o capítulo 20 de outros.</p>
				</div>
			</div>
		</div>
		
		<!-- Insight principal -->
		<div class="bg-gradient-to-r from-yellow-500/20 to-orange-500/20 backdrop-blur-sm rounded-xl lg:rounded-2xl p-2 md:p-3 border border-yellow-300/30">
			<h3 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center justify-center">
				🎯 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">A Verdade que Ninguém Conta</span>
			</h3>
			<p class="text-xl md:text-2xl lg:text-3xl text-white/90 text-center leading-relaxed">
				"Ninguém sabe tudo. Até devs sêniores googlem coisas básicas. <br>
				<strong>O segredo é saber fazer as perguntas certas.</strong>"
			</p>
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
			font-size: 1.875rem; /* text-3xl */
		}
		.slide-content h3 {
			font-size: 1.125rem; /* text-lg */
		}
		.slide-content p {
			font-size: 0.875rem; /* text-sm */
		}
	}
</style>