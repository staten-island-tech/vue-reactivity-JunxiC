<template>
  <div class="home">
    <div class="card">
      <div>
        <h2>{{ animal }}</h2>
        <h3>Price: ${{ price }}</h3>
        <img class="img" :src="image" :alt="name" />
      </div>
      <ul></ul>
      <button class="btn">Add to Cart</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'cardTemplate',
  props: {
    animal: String,
    price: String,
    image: String
  }
}
</script>
