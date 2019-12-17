<script>
	export let name;
	let clickCount = 0;

	function handleClick() {
		clickCount++;
	}
</script>

<main>
	<h1>Clicki</h1>
	<p>Click count: {clickCount}</p>
	<button on:click="{() => handleClick()}">Click me</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>