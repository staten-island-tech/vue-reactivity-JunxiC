<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <body>
    <div id="app">
      <div id="nav">
        <div class="large">
          <h3 class="dot"></h3>
          <nav class="app">
            <router-link to="/">Exotic Pets</router-link>
          </nav>
          <nav class="app">
            <router-link to="/about">Cart</router-link>
          </nav>
          <h3 class="dot2"></h3>
        </div>
      </div>
      <router-view />
    </div>
  </body>
</template>

<style scoped>
.app {
  background-color: lightblue;
  margin-top: 20px;
  align-items: center;
  display: flex;
  padding: 20px;
  border-radius: 10px;
  font-size: 20px;
  align-content: center;
  border: 1px solid black;
}

.large {
  background-color: whitesmoke;
  align-content: center;
  padding: 30px;
  border-radius: 40px;
  border: 5px solid black;
  position: fixed;
  bottom: 0;
  right: 0;
}

body {
  background-color: aquamarine;
}

.dot {
  background-color: lightblue;
  border-radius: 10px;
  padding: 5px;
  margin-top: 10px;
  border: 1px solid black;
}

.dot2 {
  background-color: lightblue;
  border-radius: 10px;
  padding: 5px;
  margin-top: 20px;
  border: 1px solid black;
}
</style>
