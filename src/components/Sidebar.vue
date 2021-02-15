<template>
  <div class="sidebar">
      <div class="note-card">
          <h2 class="note-id">Note 1</h2>
          <p class="text-preview">Text1...</p>
      </div>
      <div class="note-card">
          <h2 class="note-id">Note 2</h2>
          <p class="text-preview">Text2...</p>
      </div>
      <div class="note-card">
          <h2 class="note-id">Note 3</h2>
          <p class="text-preview">Text3...</p>
      </div>
  </div>
</template>

<script>
export default {
  name: 'SideBar',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.sidebar {
  float: left;
  margin: 0 0 0 180px;
}
</style>
