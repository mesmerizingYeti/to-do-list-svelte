<script>
	import TitleBar from "./components/TitleBar.svelte";
	import ToDoItem from "./components/ToDoItem.svelte";
	import AddButton from "./components/AddButton.svelte";

	let toDoList = [{title: "First Task", description: "This is the first task"}];

	const addTask = e => {
		console.log("Adding task")
		console.log(e);
	}
</script>

<main>
	<TitleBar backgroundColor="#ff3e00" color="white" />
	{#each toDoList as toDoItem}
		<ToDoItem {...toDoItem} />
	{/each}
	<AddButton handleClick={addTask} />
</main>

<style>
	main {
		text-align: center;
		/* padding: 1em; */
		/* max-width: 240px; */
		margin: 0 auto;
		margin: 0;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>