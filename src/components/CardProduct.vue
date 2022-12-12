<template>
    <div class="card mb-3" style="max-width: 580px;">
        <div class="row g-0">
            <div class="col-md-4">
                <img :src="require('@/assets/img/'+producto.img)" class="img-fluid rounded-start" alt="...">
            </div>
            <div class="col-md-8">
                <div class="card-body contenedorBody">
                    <div class="textDetail">
                        <h3 class="card-title detailTitle">{{producto.titulo}}</h3>
                        <p class="card-text">{{producto.desc}} x <span class="text-success"><strong>$ {{producto.precio}}</strong></span></p>
                    </div>
                    <div class="buttonDetail">
                        <button class="btn btn-light">Mostra mas</button>
                        <button class="btn btn-success">La llevo de one</button>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name:'CardProduct',
    props:{
            producto:Object
     }        
}
</script>

<style scoped>
.contenedorBody{
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    row-gap: 10px;
    background-color:#f2f2f2;
    }

    .textDetail{
        width: 100%;
        padding-left: 15px;
    }

    .buttonDetail{
        width: 100%;
        display: flex;
        flex-direction: row;
        column-gap: 15px;
        justify-content: end;
    }

    .detailTitle{
        font-family: 'Sriracha', cursive;
        margin-bottom: 5px;
    }

</style>