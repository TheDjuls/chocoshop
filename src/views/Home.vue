<template>
  <div class="home">
    <navbar/>
    <b-container class="mt-5">
      <b-breadcrumb><h4>Los Productos Mas Visitados:</h4></b-breadcrumb>
        <moreVisit/>
        <br>
      <b-breadcrumb><h4>Las Mejores Tiendas:</h4></b-breadcrumb>
        <ourShops/>
        <br>
      <b-breadcrumb><h4>Solo los mejores Productos:</h4></b-breadcrumb>
      <products/>
    </b-container>
      <foot/>
  </div>
</template>

<script>

import navbar from '@/components/navbar.vue'
import foot from '@/components/foot.vue'
import moreVisit from '@/components/moreVisit.vue'
import ourShops from '@/components/ourShops.vue'
import products from '@/components/products.vue'

export default {
  name: 'home',
  components: {
    navbar,
    moreVisit,
    ourShops,
    foot,
    products
  }
}
</script>
