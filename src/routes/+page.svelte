<script>
	import Counter from './Counter.svelte';
	import * as Fluent from "fluent-svelte";
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

	<Fluent.Button>Click</Fluent.Button>
	<Fluent.Checkbox>Check</Fluent.Checkbox>
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
</style>
