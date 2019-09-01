<template>
  <div class="home">
    <navbar/>
    <b-container class="mt-5">
      <h1>Los Productos Mas Visitados:</h1>
    <moreVisit/>
    </b-container>
  </div>
</template>

<script>

import navbar from '@/components/navbar.vue'
import moreVisit from '@/components/moreVisit.vue'

export default {
  name: 'home',
  components: {
    navbar,
    moreVisit
  }
}
</script>
