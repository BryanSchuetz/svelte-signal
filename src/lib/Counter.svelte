<script>
	let count = 0;

	const increment = () => {
		count += 1;
	};
</script>

<button class="py-4 px-8 text-red-500 bg-red-500 bg-opacity-10 rounded-full border-2 border-transparent outline-none w-48 active:bg-red-500 active:bg-opacity-20" on:click={increment}>
	Clicks: {count}
</button>

<style lang="scss">
	button {
		font-family: inherit;
		font-size: inherit;
		font-variant-numeric: tabular-nums;
	}
</style>