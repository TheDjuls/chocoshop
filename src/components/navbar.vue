<template>
    <div>
       <div id="nav">
      <b-navbar toggleable="lg" type="dark" variant="dark">
        <!--Logo-->
    <b-navbar-brand to="/">ChocoShop</b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>
      <!--Botones-->
      <b-navbar-nav>
        <b-nav-item-dropdown text="Categorias">
          <b-dropdown-item v-for="(item,index) of categories" :key="index" href="#">{{item.nombre}}</b-dropdown-item>
        </b-nav-item-dropdown>

      </b-navbar-nav>
      <b-navbar-nav class="ml-auto">
        <!--Barra de Busqueda-->
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Busqueda de Productos"></b-form-input>
          <b-button  size="sm" class="mr-4 my-2 my-sm-0" type="submit">Buscar</b-button>
          </b-nav-form>
        <b-nav-item-dropdown right>
          <!-- Usuario -->
          <template slot="button-content">Usuario</template>
          <b-dropdown-item href="#">Mi Perfil</b-dropdown-item>
          <b-dropdown-item href="#">Cerrar Sesión</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
    </b-navbar>
    </div> 
    </div>
</template>

<script>
import axios from 'axios'

export default {
    name:'navbar',
    data() {
      return {
        categories:[]
      }
    },
    methods: {
      chargeCategories:function(){
         axios
            .get('https://unsanctified-grants.000webhostapp.com/v0/catalogo/categorias/getCategorias.php')
            .then(response => {
                this.categories=response.data.data;
                console.log(this.categories);
            })
     }
    },
    mounted(){
      this.chargeCategories();
    }
}
</script>