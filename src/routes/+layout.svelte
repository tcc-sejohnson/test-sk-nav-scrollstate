<script>
	import Middle from '../lib/Middle.svelte';
</script>

<main>
	<Middle>
		<slot />
	</Middle>
</main>

<style>
	main {
		height: 1000vh;
	}
</style>
