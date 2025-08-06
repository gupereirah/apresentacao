<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white mb-3 md:mb-4 drop-shadow-lg px-4">
		🎯 Dicas para Quem Está Começando
	</h1>

	<div class="max-w-xs sm:max-w-4xl md:max-w-5xl lg:max-w-6xl mx-auto space-y-3 md:space-y-4 px-4">
		<div class="grid grid-cols-1 lg:grid-cols-2 gap-3 md:gap-4">
			<!-- Antes de se formar -->
			<div class="space-y-2 md:space-y-3">
				<h3 class="text-xl md:text-2xl lg:text-3xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center">
					📚 <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">Ainda na faculdade?</span>
				</h3>
				
				<div class="bg-gradient-to-r from-blue-500/20 to-cyan-500/20 backdrop-blur-sm rounded-lg md:rounded-xl p-2 md:p-3 border border-blue-300/30">
					<div class="flex flex-col sm:flex-row items-start">
						<span class="text-lg md:text-xl mr-0 sm:mr-3 mb-2 sm:mb-0">🏗️</span>
						<div class="text-left">
							<h4 class="text-sm md:text-base font-bold text-white mb-1">Construa seu portfólio estratégico</h4>
							<p class="text-xs md:text-sm text-white/80">Projetos com README caprichado e deploy online</p>
						</div>
					</div>
				</div>
				
				<div class="bg-gradient-to-r from-teal-500/20 to-green-500/20 backdrop-blur-sm rounded-lg md:rounded-xl p-2 md:p-3 border border-teal-300/30">
					<div class="flex flex-col sm:flex-row items-start">
						<span class="text-lg md:text-xl mr-0 sm:mr-3 mb-2 sm:mb-0">💼</span>
						<div class="text-left">
							<h4 class="text-sm md:text-base font-bold text-white mb-1">Caçe um estágio</h4>
							<p class="text-xs md:text-sm text-white/80">Experiência > Salário (por enquanto!)</p>
						</div>
					</div>
				</div>
			</div>
			
			<!-- Depois de formado -->
			<div class="space-y-2 md:space-y-3">
				<h3 class="text-xl md:text-2xl lg:text-3xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center">
					🚀 <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">Já formou? E agora?</span>
				</h3>
				
				<div class="bg-gradient-to-r from-orange-500/20 to-red-500/20 backdrop-blur-sm rounded-lg md:rounded-xl p-2 md:p-3 border border-orange-300/30">
					<div class="flex flex-col sm:flex-row items-start">
						<span class="text-lg md:text-xl mr-0 sm:mr-3 mb-2 sm:mb-0">🎯</span>
						<div class="text-left">
							<h4 class="text-sm md:text-base font-bold text-white mb-1">Aceite cargos "primos" de dev</h4>
							<p class="text-xs md:text-sm text-white/80">Suporte, QA, Analista (todos levam ao dev!)</p>
						</div>
					</div>
				</div>
				
				<div class="bg-gradient-to-r from-pink-500/20 to-purple-500/20 backdrop-blur-sm rounded-lg md:rounded-xl p-2 md:p-3 border border-pink-300/30">
					<div class="flex flex-col sm:flex-row items-start">
						<span class="text-lg md:text-xl mr-0 sm:mr-3 mb-2 sm:mb-0">🔄</span>
						<div class="text-left">
							<h4 class="text-sm md:text-base font-bold text-white mb-1">Nunca pare de estudar</h4>
							<p class="text-xs md:text-sm text-white/80">Tech evolui rápido (mas não entre em pânico!)</p>
						</div>
					</div>
				</div>
			</div>
		</div>
		
		<!-- Dica especial -->
		<div class="bg-gradient-to-r from-yellow-500/20 to-orange-500/20 backdrop-blur-sm rounded-xl lg:rounded-2xl p-3 md:p-4 border border-yellow-300/30">
			<h3 class="text-xl md:text-2xl font-bold text-white mb-2 md:mb-3 text-center">
				💡 Uma Reflexão Pessoal
			</h3>
			<p class="text-lg md:text-xl text-white/90 text-center leading-relaxed">
				Qualquer oportunidade na área de tech pode ser uma porta de entrada! Eu comecei como "o cara que conserta impressora" na HP. 😂
				<br>Foi assim que consegui entrar no mundo tech. Às vezes a porta não é a que esperamos!
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