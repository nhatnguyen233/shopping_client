<template>
  <v-app>
    <v-main>
      <list-product />
    </v-main>
  </v-app>
</template>

<script>
import ListProduct from './views/ListProduct'

export default {
  name: 'App',

  components: {
    ListProduct,
  },

  data: () => ({
    //
  }),
};
</script>
