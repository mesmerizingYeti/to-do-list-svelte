<script>
	import TitleBar from "./components/TitleBar.svelte";
	import ToDoItem from "./components/ToDoItem.svelte";

	let todolist = [];
</script>

<main>
	<TitleBar backgroundColor="#ff3e00" color="white" />
	<ToDoItem title="HELLO" />
</main>

<style>
	main {
		text-align: center;
		/* padding: 1em; */
		max-width: 240px;
		margin: 0 auto;
		margin: 0;
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