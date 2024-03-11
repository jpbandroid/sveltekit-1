<script>
	import Counter from './Counter.svelte';
	import * as Fluent from "fluent-svelte";
	import "fluent-svelte/theme.css";
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

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

@import url("https://unpkg.com/fluent-svelte/theme.css");
	/* Some base styles to get things looking right. */
	:global(body) {
		background-color: var(--fds-solid-background-base);
		color: var(--fds-text-primary);
	}
	section {
		display: flex;
		flex-direction: column;
	@@ -31,4 +38,4 @@
	h1 {
		width: 100%;
	}
</style>
