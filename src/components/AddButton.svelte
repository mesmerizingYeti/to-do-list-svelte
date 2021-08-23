<script>
  export let handleClick = event => console.log(event);
</script>

<button on:click={handleClick}>
  Add
</button>

<style>
  button {
    width: 2.5em;
    height: 2.5em;
    border-radius: 1.25em;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    background-color: #40B3FF;
    color: white;
    position: sticky;
    position: absolute;
    right: 0.5em;
    bottom: 0.5em;
  }
</style>