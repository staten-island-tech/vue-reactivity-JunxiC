<template>
  <div class="home">
    <h1 v-if="graduated">{{ student }}</h1>
    <h v-else></h</h1>
  </div>
</template>

<script>
export default {
  name: 'Home',
  components: {},
  data() {
    return {
      student: 'Harry',
      graduated: false
    }
  }
}
</script>

<style>
h1 {
  color: red;
}
</style>
