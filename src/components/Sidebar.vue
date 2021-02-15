<template>
  <div class="sidebar" >
      <div class="note-card" v-for="(note, index) in notes" v-bind:key="index" >
          <label class="note-id"> {{note.id}} </label>
          <p class="text-preview"> {{note.text}} </p>
      </div>
  </div>
</template>

<script>
export default {
  name: 'SideBar',
  props: ['notes']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.sidebar {
  float: left;
  margin: 0 0 0 100px;
}
</style>
