<script>
	import Header from './Header.svelte';
	import '../app.css';

	/** @type {{children: import('svelte').Snippet}} */
	let { children } = $props();
</script>

<main class="w-dvw h-dvh">
	{@render children()}
</main>