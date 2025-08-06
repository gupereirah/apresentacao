<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white mb-3 md:mb-4 drop-shadow-lg px-4">
		💡 A Realidade de Ser Dev Sênior
	</h1>
	<div class="max-w-xs sm:max-w-4xl md:max-w-5xl lg:max-w-6xl mx-auto space-y-2 md:space-y-3 px-4">
		<!-- O que mudou -->
		<div class="bg-gradient-to-r from-blue-500/20 to-purple-500/20 backdrop-blur-sm rounded-xl lg:rounded-2xl p-3 md:p-4 border border-blue-300/30">
			<h3 class="text-xl md:text-2xl font-bold text-white mb-2 md:mb-3 flex flex-col sm:flex-row items-center justify-center">
				🔄 <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">O Que Mudou na Prática</span>
			</h3>
			<div class="grid grid-cols-1 lg:grid-cols-2 gap-3 md:gap-4">
				<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-2 md:p-3 border border-white/20">
					<h4 class="text-base md:text-lg font-bold text-white mb-1 md:mb-2 flex flex-col sm:flex-row items-center">
						👨‍🏫 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Menos Código, Mais Mentoria</span>
					</h4>
					<p class="text-xs md:text-sm text-white/80 text-left">
						Agora passo mais tempo ajudando outros devs do que escrevendo código. E isso é incrível!
					</p>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-2 md:p-3 border border-white/20">
					<h4 class="text-base md:text-lg font-bold text-white mb-1 md:mb-2 flex flex-col sm:flex-row items-center">
						🏗️ <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Planejando mais, codando menos</span>
					</h4>
					<p class="text-xs md:text-sm text-white/80 text-left">
						Hoje eu passo mais tempo pensando "como vamos fazer isso?" do que realmente fazendo. É bem legal!
					</p>
				</div>
			</div>
		</div>
		
		<!-- As responsabilidades -->
		<div class="bg-gradient-to-r from-green-500/20 to-emerald-500/20 backdrop-blur-sm rounded-xl lg:rounded-2xl p-3 md:p-4 border border-green-300/30">
			<h3 class="text-xl md:text-2xl font-bold text-white mb-2 md:mb-3 flex flex-col sm:flex-row items-center justify-center">
				🎯 <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">Novas Responsabilidades</span>
			</h3>
			<div class="grid grid-cols-1 md:grid-cols-3 gap-2 md:gap-3">
				<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 md:p-3 border border-white/20 text-center">
					<div class="text-lg md:text-xl mb-1">🧭</div>
					<h4 class="text-xs md:text-sm font-bold text-white mb-1">Tomada de Decisão</h4>
					<p class="text-xs md:text-sm text-white/80">Escolher tecnologias e definir padrões que a equipe vai seguir.</p>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 md:p-3 border border-white/20 text-center">
					<div class="text-lg md:text-xl mb-1">🌱</div>
					<h4 class="text-xs md:text-sm font-bold text-white mb-1">Desenvolvimento de Pessoas</h4>
					<p class="text-xs md:text-sm text-white/80">Ajudar outros devs a crescerem e encontrarem seu caminho.</p>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-lg p-2 md:p-3 border border-white/20 text-center">
					<div class="text-lg md:text-xl mb-1">🔥</div>
					<h4 class="text-xs md:text-sm font-bold text-white mb-1">Apagar Incêndios</h4>
					<p class="text-xs md:text-sm text-white/80">Dev sênior acaba entrando bastante em demandas mais urgentes e críticas.</p>
				</div>
			</div>
		</div>

		<!-- A realização -->
		<div class="bg-gradient-to-r from-purple-500/20 to-pink-500/20 backdrop-blur-sm rounded-xl lg:rounded-2xl p-3 md:p-4 border border-purple-300/30">
			<h3 class="text-xl md:text-2xl font-bold text-white mb-2 md:mb-3 flex flex-col sm:flex-row items-center justify-center">
				🏆 <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">A Maior Realização</span>
			</h3>
			<div class="space-y-2">
				<p class="text-base md:text-lg text-white/90 text-center leading-relaxed">
					Ver projetos que ajudei a mentorar chegando em produção e fazendo diferença na vida das pessoas.
				</p>
				<p class="text-sm md:text-base text-white/80 text-center leading-relaxed">
					É bem legal saber que aquele código que revisamos juntos ou aquela arquitetura que discutimos 
					está sendo usado por pessoas reais no dia a dia.
				</p>
				<p class="text-sm md:text-base text-white/70 text-center">
					Acho que essa é uma das partes mais gratificantes de ser dev sênior 😊
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
			font-size: 1.5rem; /* text-2xl */
		}
		.slide-content h3 {
			font-size: 1.125rem; /* text-lg */
		}
		.slide-content p {
			font-size: 0.75rem; /* text-xs */
		}
	}
</style>