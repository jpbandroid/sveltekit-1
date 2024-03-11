<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import { Button, Checkbox } from "fluent-svelte";
</script>

<svelte:head>
	<title>Iota - ET's test site</title>
	<meta name="description" content="ErrorTek's Test Site" />
</svelte:head>

<section>
	<h1>

		Welcome to ET's testing ground!
	</h1>

	<h2>
		(non-testing website is at https://errortek.vercel.app)
	</h2>

	<Counter />

	<Button>Click</Button>
	<Checkbox>Check</Checkbox>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
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
