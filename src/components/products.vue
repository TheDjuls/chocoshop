<template>
    <div>
        <hr>
        <b-container class="bv-example-row">
  <b-row>
    <b-card v-for="(item,index) of productos" :key="index"
    :title="item.author"
    :img-src="item.download_url"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 20rem;"
    class="mb-2 ml-2"
  >
    <b-card-text>
      <span>$500</span>
    </b-card-text>

    <b-button href="#" variant="success">Añadir Al Carrito</b-button>
  </b-card>
  </b-row>

</b-container>
    </div>
</template>

<script>
import axios from 'axios'
export default {
    name:'products',
    data() {
        return {
            productos:[]
        }
    },
    methods: {
     chargeProducts:function(){
         axios
            .get('https://picsum.photos/v2/list')
            .then(response => {
                this.productos=response.data;
            })
     }
    },
     mounted(){
        this.chargeProducts(); 
     }
}
</script>

<style  scoped>
b-card{
    padding: 4%;
}
</style>