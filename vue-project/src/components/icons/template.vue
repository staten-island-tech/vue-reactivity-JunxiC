<template>
  <div class="home">
    <div class="card">
      <div>
        <h2>{{ animal }}</h2>
        <h3>Price: ${{ price }}</h3>
        <img class="img" :src="image" :alt="name" />
      </div>
      <ul></ul>
      <button
        class="btn"
        @click="
          addtocart({
            animal: animal,
            price: price,
            image: image
          })
        "
      >
        Add to Cart
      </button>
    </div>
  </div>
</template>

<script>
import { reactive } from 'vue'
export default {
  name: 'cardTemplate',
  props: {
    animal: String,
    price: String,
    image: String
  },
  methods: {
    addtocart(object) {
      cart.push(object)
      console.log(cart)
    }
  }
}
export const cart = reactive([])
</script>
