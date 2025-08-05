# 📋 Guia dos Slides da Apresentação

## 📁 Estrutura dos Arquivos

Cada slide da apresentação está em um arquivo separado na pasta `src/slides/`:

```
src/slides/
├── Slide01.svelte  # Slide de boas-vindas
├── Slide02.svelte  # Slide com lista
├── Slide03.svelte  # Slide com duas colunas
├── Slide04.svelte  # Slides 4-19 (template básico)
├── ...
└── Slide20.svelte  # Slide final de agradecimento
```

## ✏️ Como Editar um Slide

### 1. Abra o arquivo do slide que deseja editar
Exemplo: `src/slides/Slide05.svelte`

### 2. Estrutura básica de um slide:
```svelte
<script>
	export let isActive = false;
	// Adicione lógica específica do slide aqui
</script>

<div class="slide-content">
	<h1 class="text-6xl font-bold text-white mb-8 drop-shadow-lg">
		Título do Slide
	</h1>
	<p class="text-2xl text-white/90 leading-relaxed drop-shadow">
		Conteúdo principal do slide
	</p>
	
	<!-- Adicione elementos personalizados aqui -->
</div>

<style>
	.slide-content {
		@apply text-center;
	}
</style>
```

## 🎨 Exemplos de Layouts

### Slide com Lista (como Slide02)
```svelte
<ul class="text-xl text-white/90 space-y-4">
	<li class="flex items-center">
		<span class="text-2xl mr-4">📋</span>
		Seu tópico aqui
	</li>
</ul>
```

### Slide com Duas Colunas (como Slide03)
```svelte
<div class="grid grid-cols-2 gap-12 max-w-5xl mx-auto">
	<div class="bg-white/10 backdrop-blur-sm rounded-2xl p-8 border border-white/20">
		<h3 class="text-3xl font-bold text-white mb-6">Coluna 1</h3>
		<!-- Conteúdo da coluna 1 -->
	</div>
	<div class="bg-white/10 backdrop-blur-sm rounded-2xl p-8 border border-white/20">
		<h3 class="text-3xl font-bold text-white mb-6">Coluna 2</h3>
		<!-- Conteúdo da coluna 2 -->
	</div>
</div>
```

### Slide com Card Central
```svelte
<div class="max-w-4xl mx-auto">
	<div class="bg-white/10 backdrop-blur-sm rounded-2xl p-12 border border-white/20">
		<p class="text-xl text-white/80 mb-6">Seu conteúdo aqui</p>
	</div>
</div>
```

## 🎯 Classes Tailwind Úteis

### Texto
- `text-6xl` - Título grande
- `text-2xl` - Texto normal
- `text-white` - Texto branco
- `text-white/90` - Texto branco com 90% opacidade
- `font-bold` - Texto em negrito
- `drop-shadow-lg` - Sombra no texto

### Layout
- `max-w-4xl mx-auto` - Container centralizado
- `grid grid-cols-2 gap-8` - Grid de 2 colunas
- `flex items-center` - Flex centralizado
- `space-y-4` - Espaçamento vertical entre elementos

### Backgrounds e Bordas
- `bg-white/10` - Fundo branco com 10% opacidade
- `backdrop-blur-sm` - Efeito blur no fundo
- `rounded-2xl` - Bordas arredondadas
- `border border-white/20` - Borda branca com 20% opacidade

### Espaçamento
- `mb-8` - Margin bottom
- `p-12` - Padding em todos os lados
- `px-6 py-3` - Padding horizontal e vertical

## 🚀 Dicas

1. **Sempre mantenha a estrutura `<div class="slide-content">`** para consistência
2. **Use emojis** para tornar os slides mais visuais: 📊 🎯 🚀 ✨ 📋
3. **Teste sempre** após editar um slide executando `npm run dev`
4. **Mantenha a legibilidade** com bom contraste de cores
5. **Use animações sutis** com classes como `transition-all duration-200`

## 📝 Exemplo Completo de Slide Personalizado

```svelte
<script>
	export let isActive = false;
</script>

<div class="slide-content">
	<h1 class="text-6xl font-bold text-white mb-8 drop-shadow-lg">
		🚀 Meus Objetivos
	</h1>
	
	<div class="grid grid-cols-3 gap-8 max-w-5xl mx-auto mb-12">
		<div class="bg-gradient-to-b from-white/20 to-white/10 backdrop-blur-sm rounded-2xl p-8 border border-white/20">
			<div class="text-4xl mb-4">🎯</div>
			<h3 class="text-2xl font-bold text-white mb-4">Objetivo 1</h3>
			<p class="text-white/90">Descrição do primeiro objetivo</p>
		</div>
		
		<div class="bg-gradient-to-b from-white/20 to-white/10 backdrop-blur-sm rounded-2xl p-8 border border-white/20">
			<div class="text-4xl mb-4">📈</div>
			<h3 class="text-2xl font-bold text-white mb-4">Objetivo 2</h3>
			<p class="text-white/90">Descrição do segundo objetivo</p>
		</div>
		
		<div class="bg-gradient-to-b from-white/20 to-white/10 backdrop-blur-sm rounded-2xl p-8 border border-white/20">
			<div class="text-4xl mb-4">🏆</div>
			<h3 class="text-2xl font-bold text-white mb-4">Objetivo 3</h3>
			<p class="text-white/90">Descrição do terceiro objetivo</p>
		</div>
	</div>
	
	<p class="text-xl text-white/80">
		💡 Pressione as setas para navegar entre os slides
	</p>
</div>

<style>
	.slide-content {
		@apply text-center;
	}
</style>
```

---

**Divirta-se criando sua apresentação! 🎉**