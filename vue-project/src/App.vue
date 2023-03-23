<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <body>
    <div id="app">
      <div id="nav">
        <div class="large">
          <nav class="app">
            <router-link to="/">Exotic Pets</router-link>
          </nav>
          <nav class="app">
            <router-link to="/about">Cart</router-link>
          </nav>
        </div>
      </div>
      <router-view />
    </div>
  </body>
</template>

<style scoped>
.app {
  background-color: red;
  margin-top: 20px;
  align-items: center;
  display: flex;
  padding: 20px;
  border-radius: 10px;
  font-size: 20px;
  align-content: center;
}

.large {
  background-color: blue;
  align-content: center;
  padding: 30px;
  border-radius: 40px;
}
body {
  background-color: aquamarine;
}
</style>
