<script>
  export let title = "";
</script>

<div class="container">
  <div class="task">
    <input type="checkbox" name="to-do-checkbox" />
    <label for="to-do-checkbox">{title}</label>
  </div>
  <button class="del-btn">Delete</button>
</div>

<style>
  input {
    margin: 0 0.5em 0 0;
    padding: 0;
  }
  button {
    margin: 0;
  }
  .container {
    margin: 1em;
    padding: 0.75em;
    border: 1px solid black;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }
  .task {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
  }
</style>