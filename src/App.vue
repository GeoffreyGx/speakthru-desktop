<script setup lang="ts">
import Sidebar from "./components/Sidebar.vue";
</script>

<template>
  <div class="app">
    <Sidebar />
    <div class="pages">
      <router-view></router-view>
    </div>
  </div>
</template>

<style lang="scss">
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: 'Fira sans', sans-serif;
}

button {
	cursor: pointer;
	appearance: none;
	border: none;
	outline: none;
	background: none;
}

.app {
  display: flex;
  main {
    flex: 1 1 0;
    padding: 2rem;
  }

  .pages {
    margin-left: 300px;
  }
}
</style>