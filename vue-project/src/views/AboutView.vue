<template>
  <div>
    <cardTemplates
      v-for="animal in cart"
      :key="animal"
      :animal="animal.animal"
      :price="animal.price"
      :image="animal.image"
    />
  </div>
</template>

<script>
import { cart } from '../components/icons/template.vue'
import cardTemplates from '../components/icons/templates.vue'
export default {
  components: { cardTemplates },
  data() {
    return {
      cart
    }
  }
}
</script>

<style>
.about {
  display: flex;
  background-color: darkorchid;
  margin-right: 225px;
  padding: 20px;
  border-radius: 20px;
}

h1 {
  color: white;
}
</style>
