<template>
  <div class="home">
    <div class="card" v-for="list in exoticPets" :key="exoticPets">
      {{ exoticPets }}>
      <h2>{{ list.name }}</h2>
      <h3>Price: ${{ list.price }}</h3>
      <img :src="list.image" :alt="list.name" />
      <ul>
        <li v-for="animal in animals" :key="animal">{{ animal }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      exoticPets: [
        {
          animal: 'Kangaroo',
          price: 69999,
          image: 'https://i.ytimg.com/vi/gX1zPIck6uQ/maxresdefault.jpg'
        },
        {
          animal: 'Gorilla',
          price: 45999,
          image:
            'https://th-thumbnailer.cdn-si-edu.com/fapfc_i7Kihlq1W4SOLbLSzXn-M=/fit-in/1600x0/https://tf-cmsv2-smithsonianmag-media.s3.amazonaws.com/filer/45/e8/45e81e74-8044-4a89-a679-6d0eaa70d6fc/caters_gorilla_punch_03.jpg'
        },
        {
          animal: 'Seagull',
          price: 1999,
          image:
            'https://i.guim.co.uk/img/media/6ba30e96faa15f1aa2662f0da1974b233b2fce84/109_390_1831_1099/master/1831.jpg?width=1200&height=1200&quality=85&auto=format&fit=crop&s=15d51b434c4fdee5abb7ab57a3574f47'
        },
        {
          animal: 'Giraffe',
          price: 89999,
          image: 'https://thumbs.dreamstime.com/b/giraffe-walking-desert-48546806.jpg'
        },
        {
          animal: 'Hippo',
          price: 79999,
          image:
            'https://d.newsweek.com/en/full/2163756/hippo-mouth-open.jpg?w=1600&h=1600&q=88&f=4f1f90bebc0e9f8f9cb842f5f13f59c2'
        },
        {
          animal: 'Cheetah',
          price: 99999,
          image:
            'https://www.dutchnews.nl/wpcms/wp-content/uploads/2021/08/Newborn-cheetah-Photo-Safaripark-Beekse-Bergen-.jpg'
        },
        {
          animal: 'Owl',
          price: 25999,
          image: 'https://petapixel.com/assets/uploads/2021/10/babybarnowlfeat.jpg'
        },
        {
          animal: 'Sperm Whale',
          price: 345999,
          image:
            'https://www.thoughtco.com/thmb/tfdlgDz0X0Rl65HQn-w29eLZsu4=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/GettyImages-114809316-2189a0ec59b94bdea682646e19613174.jpg'
        },
        {
          animal: 'Naked Mole Rat',
          price: 39999,
          image:
            'https://static.scientificamerican.com/sciam/cache/file/18EFE41A-3592-40DF-A4AACD086FF806EE_source.jpg?w=590&h=800&4BEE41BF-B372-4950-9A9C3A8E2A898C2A'
        }
      ]
    }
  }
}
</script>

<style>
h1 {
  color: red;
}
</style>

<style>
.home {
  min-height: 100vh;
  display: flex;
  align-items: center;
}
</style>
