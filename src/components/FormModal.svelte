<script>
  export let isOpen = false;
</script>

<!-- Mask -->
<div class="mask"></div>
<!-- Modal -->
<div class={isOpen ? "modal" : "modal hidden"}>
  <form>
    <input type="text" name="title" />
    <label for="title">Title</label>
    <textarea name="description" id="description" />
    <button class="addBtn">Add Task</button>
    <button class="cancelBtn">Cancel</button>
  </form>
</div>

<style>
  .modal {
    background-color: blueviolet;
  }
  .hidden {
    display: none;
  }
</style>