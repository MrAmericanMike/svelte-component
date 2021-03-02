<svelte:options tag="hello-svelte" />

<script>
	export let _data = JSON.stringify({ cheer: "World" });
	let data = JSON.parse(_data);
</script>

<main>
	<h1>¡Hello {data.cheer}!</h1>
</main>

<style>
	main {
		text-align: center;
		color: aliceblue;
	}
	h1 {
		color: royalblue;
		text-transform: uppercase;
		font-size: 6em;
	}
</style>
