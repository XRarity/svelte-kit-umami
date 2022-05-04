<script context="module">
	export const prerender = true;
</script>

<script>
	import Counter from '$lib/Counter.svelte';
	import { UmamiAnalytics } from '@sveltinio/services';
</script>

<svelte:head>
	<title>Umami Public Analytics</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<UmamiAnalytics
 websiteID="4f5c2742-a1dd-4695-95a7-8bde8b75f386"
 srcURL="https://umami-production-ed79.up.railway.app/umami.js"
/>

<section>
	<h1>
		<!-- <div class="welcome">
			<picture>
				<source srcset="svelte-welcome.webp" type="image/webp" />
				<img src="svelte-welcome.png" alt="Welcome" />
			</picture>
		</div> -->

		App with Umami Public Analytics
	</h1>

	<!-- <h2>
		try editing <strong>src/routes/index.svelte</strong>
	</h2> -->

	<!-- <Counter /> -->
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
