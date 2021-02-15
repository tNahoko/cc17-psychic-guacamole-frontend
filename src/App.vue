<template>
  <div id="app">
    <h1 class="header">Notes App</h1>
    <div class="main-body">
      <Sidebar v-bind:notes="notes" />
      <NoteSpace />
    </div>
  </div>
</template>

<script>
import Sidebar from './components/Sidebar.vue'
import NoteSpace from './components/NoteSpace.vue'
import axios from 'axios';

export default {
  name: 'App',
  components: {
    Sidebar,
    NoteSpace
  },
  data() {
    return {
      notes: []
    }
  },
  methods: {
    showNote: async function () {

    },
    addNote: async function () {

    },
    deleteNote: async function () {

    }
  },
  async created() {
    try {
      const response = await axios.get('https://pg-note-backend.herokuapp.com/api/notes');
      this.notes = response.data;
    } catch (err) {
      console.log(err);
    }
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
