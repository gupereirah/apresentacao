<script>
	import '../app.css';
	
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" type="image/svg+xml" href="/favicon.svg" />
	<link rel="alternate icon" href="/favicon.svg" />
	<title>Apresentação</title>
</svelte:head>

<main class="w-full h-full">
	{@render children?.()}
</main>

<style>
	:global(html, body) {
		margin: 0;
		padding: 0;
		width: 100%;
		height: 100%;
		overflow: hidden;
	}
</style>
