<script>
	export const isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-6 md:mb-8 drop-shadow-lg px-4">
		🎓 Início da Trajetória
	</h1>
	<p class="text-xl md:text-2xl lg:text-3xl text-white/90 leading-relaxed drop-shadow mb-8 md:mb-12 px-4">
		Primeiros passos no mundo da tecnologia
	</p>
	
	<div class="max-w-xs sm:max-w-3xl md:max-w-4xl lg:max-w-full mx-auto px-4">
		<div class="bg-white/10 backdrop-blur-sm rounded-2xl md:rounded-3xl p-6 md:p-8 lg:p-12 border border-white/20">
			<div class="grid grid-cols-1 lg:grid-cols-2 gap-8 lg:gap-12">
				<div class="text-left">
					<h3 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-4 md:mb-6 flex flex-col sm:flex-row items-start sm:items-center">
						🏫 <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">Formação Base</span>
					</h3>
					<ul class="text-xl md:text-2xl lg:text-4xl text-white/90 space-y-3 md:space-y-4">
						<li class="flex items-start">
							<span class="text-2xl md:text-4xl mr-3 md:mr-4 mt-1">📚</span>
							<div>
								<strong>Ensino Médio Técnico</strong><br>
								<span class="text-lg md:text-2xl text-white/70">Colégio Módulo (2009-2011)</span>
							</div>
						</li>
						<li class="flex items-start">
							<span class="text-2xl md:text-4xl mr-3 md:mr-4 mt-1">💭</span>
							<div>
								Optei pelo técnico em tecnologia<br>
								<span class="text-lg md:text-2xl text-white/70">Área de curiosidade e interesse, mas sem conhecer a realidade</span>
							</div>
						</li>
					</ul>
				</div>
				
				<div class="text-left">
					<h3 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-4 md:mb-6 flex flex-col sm:flex-row items-start sm:items-center">
						🏢 <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">Primeira Experiência</span>
					</h3>
					<ul class="text-xl md:text-2xl lg:text-4xl text-white/90 space-y-3 md:space-y-4">
						<li class="flex items-start">
							<span class="text-2xl md:text-4xl mr-3 md:mr-4 mt-1">👨‍💼</span>
							<div>
								<strong>Estagiário na HP</strong><br>
								<span class="text-lg md:text-2xl text-white/70">Primeira oportunidade profissional, depois efetivado</span>
							</div>
						</li>
						<li class="flex items-start">
							<span class="text-2xl md:text-4xl mr-3 md:mr-4 mt-1">🔧</span>
							<div>
								Instalação e manutenção<br>
								<span class="text-lg md:text-2xl text-white/70">Impressoras e servidores</span>
							</div>
						</li>
					</ul>
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
			font-size: 2.25rem; /* text-4xl */
		}
		.slide-content h3 {
			font-size: 1.25rem; /* text-xl */
		}
		.slide-content ul {
			font-size: 1rem; /* text-base */
		}
	}
</style>