<script>
  export let color = "white";
  export let backgroundColor = "blue";
</script>

<div class="container" 
  style={`background-color: ${backgroundColor}; color: ${color}`}
>
  <h1>To Do List in Svelte</h1>
  <a href="https://github.com/mesmerizingYeti/to-do-list-svelte">
    <i class="fab fa-github fa-2x"></i>
  </a>
</div>

<style>
  a {
    color: white;
    border-radius: 50%;
    height: 3em;
    width: 3em;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  a:hover {
    background-color: rgba(255, 255, 255, 0.15);
  }
  .container {
    height: 4em;
    margin: 0;
    padding: 0.5em 1.5em;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }
</style>