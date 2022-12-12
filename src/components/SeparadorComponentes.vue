<template>
    <div class="container separador">
        <h1 class="text-center p-1">{{ titulo1 }}</h1>
        <h3 class="text-center p-1">{{ titulo2 }}</h3>
    </div>
</template>

<script>
export default {
    name:'SeparadorComponentes',
    props:{
        titulo1:String,
        titulo2:String
    }

}
</script>

<style scoped>
    .separador{
        background-color: yellowgreen;
    }
</style>