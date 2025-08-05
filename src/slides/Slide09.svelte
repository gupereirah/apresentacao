<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-4xl font-bold text-white mb-4 drop-shadow-lg">
		📈 A Evolução Continua
	</h1>
	
	<div class="max-w-6xl mx-auto space-y-4">
		<!-- Marcos da evolução -->
		<div class="bg-gradient-to-r from-blue-500/20 to-purple-500/20 backdrop-blur-sm rounded-3xl p-4 border border-blue-300/30">
			<h3 class="text-xl font-bold text-white mb-4 flex items-center justify-center">
				🌱 <span class="ml-3">Nossa Jornada de Crescimento</span>
			</h3>
			<div class="grid grid-cols-3 gap-4">
				<div class="bg-white/10 backdrop-blur-sm rounded-xl p-3 border border-white/20 text-center">
					<div class="text-2xl mb-2">🌱</div>
					<h4 class="text-base font-bold text-white mb-1">Dev Júnior</h4>
					<p class="text-xs text-white/80 mb-2">"Como isso funciona?"</p>
					<ul class="text-xs text-white/70 space-y-1 text-left">
						<li>• Aprendendo sintaxe</li>
						<li>• Seguindo tutoriais</li>
						<li>• Medo de quebrar coisas</li>
					</ul>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-xl p-3 border border-white/20 text-center">
					<div class="text-2xl mb-2">🌿</div>
					<h4 class="text-base font-bold text-white mb-1">Dev Pleno</h4>
					<p class="text-xs text-white/80 mb-2">"Por que isso funciona?"</p>
					<ul class="text-xs text-white/70 space-y-1 text-left">
						<li>• Entendendo padrões</li>
						<li>• Resolvendo problemas</li>
						<li>• Começando a ensinar</li>
					</ul>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-xl p-3 border border-white/20 text-center">
					<div class="text-2xl mb-2">🌳</div>
					<h4 class="text-base font-bold text-white mb-1">Dev Sênior</h4>
					<p class="text-xs text-white/80 mb-2">"Como fazer funcionar melhor?"</p>
					<ul class="text-xs text-white/70 space-y-1 text-left">
						<li>• Arquitetando soluções</li>
						<li>• Mentorando outros</li>
						<li>• Pensando no negócio</li>
					</ul>
				</div>
			</div>
		</div>
		
		<!-- Insights e lições em duas colunas -->
		<div class="grid grid-cols-2 gap-6">
			<!-- As lições mais importantes -->
			<div class="bg-gradient-to-r from-green-500/20 to-emerald-500/20 backdrop-blur-sm rounded-3xl p-5 border border-green-300/30">
				<h3 class="text-xl font-bold text-white mb-4 flex items-center justify-center">
					💡 <span class="ml-2">Lições Importantes</span>
				</h3>
				<div class="space-y-4">
					<div class="bg-white/10 backdrop-blur-sm rounded-xl p-4 border border-white/20">
						<h4 class="text-base font-bold text-white mb-2 flex items-center">
							🧠 <span class="ml-2">Soft > Hard Skills</span>
						</h4>
						<p class="text-sm text-white/80 text-left">
							Comunicação e trabalho em equipe superam conhecer 20 frameworks.
						</p>
					</div>
					
					<div class="bg-white/10 backdrop-blur-sm rounded-xl p-4 border border-white/20">
						<h4 class="text-base font-bold text-white mb-2 flex items-center">
							🎓 <span class="ml-2">Ensinar é Aprender</span>
						</h4>
						<div class="text-sm text-white/80 text-left space-y-2">
							<p><strong>Duck Debugging:</strong></p>
							<p class="italic">"Explicar para um pato me fez achar bugs que horas de debug não acharam."</p>
						</div>
					</div>
				</div>
			</div>
			
			<!-- O que permanece -->
			<div class="bg-gradient-to-r from-purple-500/20 to-pink-500/20 backdrop-blur-sm rounded-3xl p-5 border border-purple-300/30">
				<h3 class="text-xl font-bold text-white mb-4 text-center">
					🎯 O Que Nunca Muda
				</h3>
				<div class="bg-white/10 backdrop-blur-sm rounded-xl p-4 border border-white/20">
					<p class="text-base text-white/90 text-center leading-relaxed">
						A curiosidade, a vontade de aprender e o receio de dar errado. 😅
					</p>
					<p class="text-sm text-white/80 text-center mt-3">
						<strong>Aceite isso como parte da jornada!</strong>
					</p>
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