<script>
  export let isOpen = false;

  const handleCancel = e => {
    isOpen = false;
  };
</script>

<!-- Mask -->
<div class="mask"></div>
<!-- Modal -->
<div class={isOpen ? "modal" : "modal hidden"}>
  <form>
    <div class="column">
      <label for="title">Title</label>
      <input type="text" name="title" id="title" />
      <textarea name="description" id="description" />
      <button class="addBtn">Add Task</button>
      <button class="cancelBtn" on:click={handleCancel}>Cancel</button>
    </div>
  </form>
</div>

<style>
  .modal {
    background-color: blueviolet;
    position: absolute;
  }
  .hidden {
    display: none;
  }
</style>