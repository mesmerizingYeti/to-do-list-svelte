<script>
  export let title = "";
  export let description = "";
  let finished = false;

  const handleChange = e => finished = e.target.checked;

  const handleBtnClick = e => {
    console.log(e);
  };

</script>

<div class={finished ? "container finished" : "container"}>
  <div class="task">
    <input type="checkbox" name="to-do-checkbox" on:change={handleChange}/>
    <label 
      for="to-do-checkbox"
      class={finished ? "cross-out" : ""}
    >
      {title}
    </label>
    <p>
      {description}
    </p>
  </div>
  <button class="del-btn" on:click={handleBtnClick}>
    <span class="icon-container">
      <i class="fas fa-trash-alt fa-lg"></i>
    </span>
  </button>
</div>

<style>
  input {
    margin: 0 0.5em 0 0;
    padding: 0;
  }
  label {
    user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    -khtml-user-select: none;
    -webkit-user-select: none;
    -webkit-touch-callout: none;
    font-size: 1.5em;
  }
  p {
    margin: 0 0 0 2em;
  }
  button {
    margin: 0;
    padding: 0.5em;
    background-color: transparent;
    border: none;
    border-radius: 0.5em;
  }
  button:hover {
    background-color: rgba(167, 97, 97, 0.2);
  }
  button:active {
    background-color: rgba(167, 97, 97, 0.3);
  }
  .finished {
    color: white;
    background-color: #676778 ;
    text-decoration: line-through;
  }
  .container {
    margin: 1em;
    padding: 0.75em;
    border: 1px solid black;
    border-radius: 0.25em;
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
    align-content: center;
  }
  .icon-container {
    color: #cb4154;
  }
  
</style>