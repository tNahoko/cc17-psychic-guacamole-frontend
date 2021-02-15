<template>
  <div id="app">
    <h1 class="app-title">Notes app</h1>
    <div class="main-body">
      <Sidebar />
      <NoteSpace />
    </div>
  </div>
</template>

<script>
import Sidebar from './components/Sidebar.vue'
import NoteSpace from './components/NoteSpace.vue'

export default {
  name: 'App',
  components: {
    Sidebar,
    NoteSpace
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.main-body {
  display: flex;
}
</style>
