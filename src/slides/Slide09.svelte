<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white mb-3 md:mb-4 drop-shadow-lg px-4">
		📈 A Evolução Continua
	</h1>
	
	<div class="max-w-xs sm:max-w-4xl md:max-w-5xl lg:max-w-6xl mx-auto space-y-3 md:space-y-4 px-4">
		<!-- Marcos da evolução -->
		<div class="bg-gradient-to-r from-blue-500/20 to-purple-500/20 backdrop-blur-sm rounded-2xl md:rounded-3xl p-3 md:p-4 border border-blue-300/30">
			<h3 class="text-xl md:text-2xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center justify-center">
				🌱 <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">Nossa Jornada de Crescimento</span>
			</h3>
			<div class="grid grid-cols-1 md:grid-cols-3 gap-3 md:gap-4">
				<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-2 md:p-3 border border-white/20 text-center">
					<div class="text-xl md:text-2xl mb-1 md:mb-2">🌱</div>
					<h4 class="text-base md:text-lg font-bold text-white mb-1">Dev Júnior</h4>
					<p class="text-xs md:text-sm text-white/80 mb-2">"Como isso funciona?"</p>
					<ul class="text-xs md:text-sm text-white/70 space-y-1 text-left">
						<li>• Aprendendo sintaxe</li>
						<li>• Seguindo tutoriais</li>
						<li>• Medo de quebrar coisas</li>
					</ul>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-2 md:p-3 border border-white/20 text-center">
					<div class="text-xl md:text-2xl mb-1 md:mb-2">🌿</div>
					<h4 class="text-base md:text-lg font-bold text-white mb-1">Dev Pleno</h4>
					<p class="text-xs md:text-sm text-white/80 mb-2">"Por que isso funciona?"</p>
					<ul class="text-xs md:text-sm text-white/70 space-y-1 text-left">
						<li>• Entendendo padrões</li>
						<li>• Resolvendo problemas</li>
						<li>• Começando a ensinar</li>
					</ul>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-2 md:p-3 border border-white/20 text-center">
					<div class="text-xl md:text-2xl mb-1 md:mb-2">🌳</div>
					<h4 class="text-base md:text-lg font-bold text-white mb-1">Dev Sênior</h4>
					<p class="text-xs md:text-sm text-white/80 mb-2">"Como fazer funcionar melhor?"</p>
					<ul class="text-xs md:text-sm text-white/70 space-y-1 text-left">
						<li>• Arquitetando soluções</li>
						<li>• Mentorando outros</li>
						<li>• Pensando no negócio</li>
					</ul>
				</div>
			</div>
		</div>
		
		<!-- Insights e lições em duas colunas -->
		<div class="grid grid-cols-1 lg:grid-cols-2 gap-4 md:gap-6">
			<!-- As lições mais importantes -->
			<div class="bg-gradient-to-r from-green-500/20 to-emerald-500/20 backdrop-blur-sm rounded-2xl md:rounded-3xl p-4 md:p-5 border border-green-300/30">
				<h3 class="text-xl md:text-2xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center justify-center">
					💡 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Lições Importantes</span>
				</h3>
				<div class="space-y-3 md:space-y-4">
					<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-3 md:p-4 border border-white/20">
						<h4 class="text-base md:text-lg font-bold text-white mb-1 md:mb-2 flex flex-col sm:flex-row items-center">
							🧠 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Soft > Hard Skills</span>
						</h4>
						<p class="text-sm md:text-base text-white/80 text-left">
							Comunicação e trabalho em equipe superam conhecer 20 frameworks.
						</p>
					</div>
					
					<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-3 md:p-4 border border-white/20">
						<h4 class="text-base md:text-lg font-bold text-white mb-1 md:mb-2 flex flex-col sm:flex-row items-center">
							🎓 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Ensinar é Aprender</span>
						</h4>
						<div class="text-sm md:text-base text-white/80 text-left space-y-2">
							<p><strong>Duck Debugging:</strong></p>
							<p class="italic">"Explicar para um pato me fez achar bugs que horas de debug não acharam."</p>
						</div>
					</div>
				</div>
			</div>
			
			<!-- O que permanece -->
			<div class="bg-gradient-to-r from-purple-500/20 to-pink-500/20 backdrop-blur-sm rounded-2xl md:rounded-3xl p-4 md:p-5 border border-purple-300/30">
				<h3 class="text-xl md:text-2xl font-bold text-white mb-3 md:mb-4 text-center">
					🎯 O Que Nunca Muda
				</h3>
				<div class="bg-white/10 backdrop-blur-sm rounded-lg md:rounded-xl p-3 md:p-4 border border-white/20">
					<p class="text-base md:text-lg text-white/90 text-center leading-relaxed">
						A curiosidade, a vontade de aprender e o receio de dar errado. 😅
					</p>
					<p class="text-sm md:text-base text-white/80 text-center mt-3">
						<strong>Aceite isso como parte da jornada!</strong>
					</p>
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