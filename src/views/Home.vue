<template>
  <div class="home">
    <navbar/>
    <b-container class="mt-5">
      <b-breadcrumb><h4>Los Productos Mas Visitados:</h4></b-breadcrumb>
        <moreVisit/>
        <br>
      <b-breadcrumb><h4>Las Mejores Tiendas:</h4></b-breadcrumb>
        <ourShops/>
    </b-container>
      <foot/>
  </div>
</template>

<script>

import navbar from '@/components/navbar.vue'
import foot from '@/components/foot.vue'
import moreVisit from '@/components/moreVisit.vue'
import ourShops from '@/components/ourShops.vue'

export default {
  name: 'home',
  components: {
    navbar,
    moreVisit,
    ourShops,
    foot
  }
}
</script>
