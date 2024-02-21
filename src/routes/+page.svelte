<script>
	let count = 0;

	function increment() {
		count += 1;
	}

	function decrement() {
		count -= 1;
	}
</script>

<div class="font-bold flex flex-col items-center justify-center h-screen bg-yellow-300">
	<h1 class="container text-6xl">Counter-Website</h1>
	<p class="text-4xl">{count}</p>
	<div class="flex space-x-4">
		<button
			class="bg-green-500 hover:bg-green-700 text-white py-2 px-4 rounded"
			on:click={increment}
		>
			Increment
		</button>

		<button class="bg-red-500 hover:bg-red-700 text-white py-2 px-4 rounded" on:click={decrement}>
			Decrement
		</button>
	</div>
</div>
