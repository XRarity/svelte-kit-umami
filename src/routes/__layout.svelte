<script>
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
	import { browser } from '$app/env';
</script>

{#if browser}
	<script async defer data-website-id="4f5c2742-a1dd-4695-95a7-8bde8b75f386" src="https://umami-production-ed79.up.railway.app/umami.js"></script>
{/if}

<Header />

<main>
	<slot />
</main>

<!-- <footer>
	<p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p>
</footer> -->

<style>
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 1024px;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 40px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 40px 0;
		}
	}
</style>
