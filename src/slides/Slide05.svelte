<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-6xl font-bold text-white mb-8 drop-shadow-lg">
		🎯 Primeiro Grande Desafio
	</h1>

	<div class="max-w-6xl mx-auto space-y-8">
		<!-- Desafio proposto -->
		<div class="bg-gradient-to-r from-red-500/20 to-orange-500/20 backdrop-blur-sm rounded-3xl p-10 border border-red-300/30">
			<h3 class="text-4xl font-bold text-white mb-6 flex items-center justify-center">
				⚡ <span class="ml-3">Desafio Proposto</span>
			</h3>
			<p class="text-2xl text-white/90 text-center mb-8">
				"Automatizar testes na empresa"
			</p>
			
			<div class="grid grid-cols-2 gap-8">
				<div class="bg-white/10 backdrop-blur-sm rounded-2xl p-6 border border-white/20">
					<h4 class="text-xl font-bold text-white mb-4 flex items-center">
						📚 <span class="ml-2">Curso QA Academy</span>
					</h4>
					<ul class="text-lg text-white/90 space-y-2 text-left">
						<li>• Java</li>
						<li>• Selenium</li>
						<li>• Gherkin</li>
					</ul>
				</div>
				
				<div class="bg-white/10 backdrop-blur-sm rounded-2xl p-6 border border-white/20">
					<h4 class="text-xl font-bold text-white mb-4 flex items-center">
						😰 <span class="ml-2">Primeira Dificuldade</span>
					</h4>
					<p class="text-lg text-white/90 text-left">
						<strong>Lógica de programação</strong><br>
						<span class="text-white/70">Não entendia como as coisas funcionavam de fato aplicadas</span>
					</p>
				</div>
			</div>
		</div>
		
		<div class="text-center">
			<div class="inline-block bg-green-500/20 backdrop-blur-sm rounded-2xl px-8 py-4 border border-green-300/30">
				<p class="text-xl text-white font-semibold">
					✅ <strong>Resultado:</strong> Consegui desenvolver automações!
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