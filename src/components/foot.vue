<template>
<div>
<div class="font-small pt-4 mt-4 bg-dark">
    <b-container class="text-left">
      <b-row>
        <b-col sm="6">
          <h5 class="title">ChocoShop</h5>
          <p>Chocoshop es una empresa tabasqueña dedicada a las ventas en linea dentro de la entidad</p>
        </b-col>
        <b-col sm="6">
          <h5 class="title">Links</h5>
          <ul>
            <li class="list-unstyled"><a href="#!">Categorias</a></li>
          </ul>
        </b-col>
      </b-row>
    </b-container>
    <div class="footer-copyright text-center py-3">
      <b-container fluid>
        &copy; 2019 Copyright: <a to="/"> ChocoShop.com </a>
      </b-container>
    </div>
  </div>
</div>
</template>

<script>
export default {
    name:'foot'
}
</script>

<style scoped>
*{
    color: white;
}
</style>