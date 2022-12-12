<template>
  <div class="container">
        <div class="tituloListado">
            <h1 class="titulo">Anda Pidiendo, dale que ia prendimo'el horno!!!</h1>
        </div>
        <div class="contenedorListado">
            <CardProduct v-for="(prod,i) of productos" :key="i" :producto="prod"></CardProduct>
        </div>
    </div>
</template>

<script>
import CardProduct from './CardProduct.vue'

export default {
    name:'ProductList',
    components:{
        CardProduct
    },
     props:{
            productos:Array
     }        
    

}
</script>

<style scoped>
    .contenedorListado{
        padding: 20px;
        display:flex;
        flex-direction: row;
        flex-wrap: wrap;
        column-gap: 20px;
        row-gap: 5px;
        justify-content:center;
    }

    .titulo{
        margin: 25px;
        font-family: 'Sriracha', cursive;
        text-align: center;
    }
</style>