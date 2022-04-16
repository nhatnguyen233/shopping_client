<template>
  <div id="list-product">
    <div v-for="item in listProducts" :key="item.id">
      <product-card :product="item" />
    </div>
  </div>
</template>

<script>
import ProductCard from '../../components/ProductCard.vue'

export default {
  components: { ProductCard },
  data: () => ({
    listProducts: [
      {
        id: 1,
        thumbnail: 'https://cdn.vuetifyjs.com/images/cards/cooking.png',
        title: 'Cafe Badilico',
        review: {
          rate: 4.5,
          count: 413
        },
        address: 'Italian, Cafe',
        description: 'Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.',
        available_time: [
          '17:30',
          '19:30',
          '20:00',
          '21:00'
        ]
      }
    ]
  }),

  methods: {
  },
}

</script>