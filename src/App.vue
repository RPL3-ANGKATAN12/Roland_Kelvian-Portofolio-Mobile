<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <img src="@/assets/logo.svg" height="40" />
    <div class="menu">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/project">Project</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
    </div>
  </header>
  <RouterView />
</template>

<style scoped>
header {
  width: 100vw;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: gray;
}

.menu * {
  text-decoration: none;
  margin-right: 10px;
  color: black;
}
</style>