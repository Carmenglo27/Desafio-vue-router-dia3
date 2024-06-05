<template>
    <div class="productos">
      <h1>Productos</h1>
      <div>
        <p>Nombre: {{ nombre }}</p>
        <p>Descripcion: {{ descripcion }}</p>
        <p>Precio: {{ precio }}</p>
        <p>Cantidad: {{ cantidad }}</p>
        <div class="inicio-productos">
        <router-link class="btn btn-success" to="/">Volver al inicio</router-link>
        </div>
        </div>
    </div>
</template>

<script>


export default {
    name: 'ProductosView',
    props: {
        nombre: String,
        descripcion: String,
        precio: Number,
        cantidad: Number,
    }
    
}
</script>

<style>
.productos{
  padding-top: 150px;
  padding-left: 50px;
}

.inicio-productos{
    padding-left: 5px;
}

.btn{
    background-color: palevioletred;
}
</style>