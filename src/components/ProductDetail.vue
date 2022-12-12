<template>
  <div class="container contenedorPrincipal">
        <div class="card mb-3" style="max-width: 100%;">
            <div class="row g-0">
                <div class="col-md-6">
                    <img :src="require('@/assets/img/'+product.img)" class="img-fluid rounded-start" alt="...">
                </div>
                <div class="col-md-6">
                    <div class="card-body contenedorBody">
                        <div class="textDetail">
                            <div class="detailTitle">
                                <h2>{{product.titulo}}</h2>
                            </div>
                            <div class="detailSubTitle">
                                <h5>{{product.desc}} x <span class="text-success"><strong>$ {{product.precio}}</strong></span></h5>
                            </div>
                            <div class="detailText">
                                <p>{{product.info1}}</p>
                                <p>{{product.info2}}</p>
                                <p>{{product.info3}}</p>
                            </div>
                        </div>
                        <div class="buttonDetail">
                            <button class="btn btn-light">Hmmm voy a ve'otra</button>
                            <button class="btn btn-success">La quiero iaaaaa!</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ProductDetail',
    props:{
        product:Object,
    }
}
</script>

<style scoped>
    .contenedorPrincipal{
    padding: 10px;
    }

    .contenedorBody{
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        row-gap: 10px;
    }

    .textDetail{
        width: 100%;
        padding-left: 15px;
    }

    .buttonDetail{
        width: 100%;
        height: 50px;
        display: flex;
        flex-direction: row;
        column-gap: 15px;
        justify-content: end;
    }

    .detailTitle{
        font-family: 'Sriracha', cursive;
        margin-bottom: 25px;
    }

    .detailSubTitle{
        margin-bottom: 25px;
    }
</style>

