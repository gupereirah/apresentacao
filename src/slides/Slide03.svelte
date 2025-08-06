<script>
	export const isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-6 md:mb-8 drop-shadow-lg px-4">
		🏥 Entrada na Febrafar
	</h1>
	<p class="text-xl md:text-2xl lg:text-3xl text-white/90 leading-relaxed drop-shadow mb-8 md:mb-12 px-4">
		O começo de uma nova jornada
	</p>
	
	<div class="max-w-xs sm:max-w-3xl md:max-w-4xl lg:max-w-full mx-auto px-4">
		<!-- Primeiro cargo -->
		<div class="bg-gradient-to-r from-blue-500/20 to-purple-500/20 backdrop-blur-sm rounded-2xl md:rounded-3xl p-6 md:p-8 lg:p-10 border border-white/30">
			<h3 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-4 md:mb-6 flex flex-col sm:flex-row items-center justify-center">
				👨‍💼 <span class="ml-0 sm:ml-3 mt-2 sm:mt-0">Assistente de Produto</span>
			</h3>
			<div class="grid grid-cols-1 lg:grid-cols-2 gap-6 lg:gap-8 text-left">
				<div>
					<h4 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-3 md:mb-4">🔍 Atividades:</h4>
					<ul class="text-xl md:text-2xl lg:text-3xl text-white/90 space-y-3 md:space-y-4">
						<li>• Validação de funcionalidades</li>
						<li>• Documentação técnica</li>
						<li>• Análise de requisitos</li>
					</ul>
				</div>
				<div>
					<h4 class="text-2xl md:text-3xl lg:text-4xl font-bold text-white mb-3 md:mb-4">🏗️ Contexto:</h4>
					<ul class="text-xl md:text-2xl lg:text-3xl text-white/90 space-y-3 md:space-y-4">
						<li>• Produtos desenvolvidos por terceiros</li>
						<li>• Ponte entre negócio e técnico</li>
						<li>• Ainda sem programação</li>
					</ul>
				</div>
			</div>
		</div>
		
		<div class="text-center">
			<p class="text-xl md:text-2xl lg:text-3xl text-white/70 max-w-4xl mx-auto leading-relaxed">
				💡 <strong>Aprendizado:</strong> Adquiri base técnica e responsabilidade, mas ainda não programava
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
			font-size: 2.25rem; /* text-4xl */
		}
		.slide-content h3 {
			font-size: 1.5rem; /* text-2xl */
		}
		.slide-content ul {
			font-size: 1rem; /* text-base */
		}
	}
</style>