<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-4 md:mb-6 drop-shadow-lg px-4">
		🚀 A Virada para Dev
	</h1>
	
	<div class="max-w-xs sm:max-w-4xl md:max-w-5xl lg:max-w-6xl mx-auto space-y-4 md:space-y-6 px-4">
		<!-- Mudança na empresa -->
		<div class="bg-gradient-to-r from-purple-500/20 to-pink-500/20 backdrop-blur-sm rounded-2xl md:rounded-3xl p-4 md:p-6 border border-purple-300/30">
			<h3 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-4 md:mb-6 text-center">
				🏢 Empresa Internalizou o Time de Desenvolvimento
			</h3>
			
			<div class="bg-yellow-500/20 backdrop-blur-sm rounded-xl lg:rounded-2xl p-4 md:p-6 border border-yellow-300/30 mb-4 md:mb-6">
				<h4 class="text-xl md:text-2xl lg:text-3xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center justify-center">
					🎯 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Novo Desafio</span>
				</h4>
				<p class="text-lg md:text-xl lg:text-2xl text-white/90 text-center">
					"Seja o primeiro Dev formado internamente"
				</p>
			</div>
			
			<div class="grid grid-cols-1 lg:grid-cols-2 gap-4 md:gap-6">
				<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-3 md:p-4 border border-white/20">
					<h4 class="text-lg md:text-xl lg:text-2xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center">
						🎓 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Código do Futuro</span>
					</h4>
					<ul class="text-lg md:text-xl text-white/90 space-y-2 text-left">
						<li>• Gama Academy</li>
						<li>• Angular</li>
						<li>• .NET</li>
					</ul>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-xl lg:rounded-2xl p-3 md:p-4 border border-white/20">
					<h4 class="text-lg md:text-xl lg:text-2xl font-bold text-white mb-3 md:mb-4 flex flex-col sm:flex-row items-center">
						📖 <span class="ml-0 sm:ml-2 mt-2 sm:mt-0">Estudo Complementar</span>
					</h4>
					<ul class="text-lg md:text-xl text-white/90 space-y-2 text-left">
						<li>• Alura</li>
						<li>• Vue/Nuxt</li>
						<li>• SvelteKit</li>
					</ul>
				</div>
			</div>
		</div>
		
		<div class="text-center">
			<div class="inline-block bg-green-500/20 backdrop-blur-sm rounded-xl lg:rounded-2xl px-6 md:px-8 py-3 md:py-4 border border-green-300/30">
				<p class="text-xl md:text-2xl text-white font-semibold">
					📈 <strong>Evolução:</strong> Dev Jr → Pleno → Sênior
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
			font-size: 1.875rem; /* text-3xl */
		}
		.slide-content h3 {
			font-size: 1.25rem; /* text-xl */
		}
		.slide-content p {
			font-size: 1rem; /* text-base */
		}
	}
</style>