<script setup>
import Header from './components/AppHeader.vue';
import HomePage from './components/HomePage.vue';
</script>
<template>
  <div class="container-fluid">
    <Header />
    <HomePage />
  </div>
</template>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
