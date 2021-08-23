<script>
  export let handleClick = event => console.log(event);
</script>

<button on:click={handleClick}>
  Add
</button>

<style>
  button {
    width: 2em;
    height: 2em;
    border-radius: 1em;
    box-shadow: black 1em;
    background-color: orange;
    color: white;
    position: sticky;
    right: -1em;
    bottom: -1em;
  }
</style>