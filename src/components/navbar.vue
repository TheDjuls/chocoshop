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
        <b-nav-item href="#">Categorias</b-nav-item>
      </b-navbar-nav>
      <b-navbar-nav class="ml-auto">
        <!--Barra de Busqueda-->
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Busqueda de Productos"></b-form-input>
          <b-button  size="sm" class="my-2 my-sm-0" type="submit">Buscar</b-button>
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
export default {
    name:'navbar'
}
</script>