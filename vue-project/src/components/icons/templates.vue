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
          removefromcart({
            animal: animal,
            price: price,
            image: image
          })
        "
      >
        Remove From Cart
      </button>
    </div>
  </div>
</template>

<script>
import { cart } from './template.vue'
export default {
  name: 'cardTemplates',
  props: {
    animal: String,
    price: String,
    image: String
  },
  methods: {
    removefromcart(object) {
      let animal = cart.find((animal) => animal.animal === object.animal)
      cart.splice(animal, 1)
      console.log(cart)
    }
  }
}
</script>
