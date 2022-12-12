<template>
  <div class="container contenedorPrincipal">
        <div class="tituloCartContainer">
            <h1 class="tituloCart">Estas a un paso del disfrute!!</h1>
            <h1 class="tituloCart">Vamooooo! que no se te olvide nada</h1>
            
        </div>
        <div class="datailCartContainer">
            <table class="table">
                <thead>
                    <tr>
                        <th scope="col">Pizza ID.</th>
                        <th scope="col">Desc.</th>
                        <th scope="col">Qty.</th>
                        <th scope="col">P.U</th>
                        <th scope="col">Importe</th>
                    </tr>
                </thead>
                <tbody class="table-group-divider">
                    <tr v-for="(item,i) of items" :key="i">
                        <td>{{item.id}}</td>
                        <td>{{item.titulo}}</td>
                        <td>{{item.qty}}</td>
                        <td>{{item.pu}}</td>
                        <td>{{item.pu}}</td>
                        <td><i class="bi bi-trash3-fill"></i></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="buttonCartContainter">
            <button class="btn btn-danger">Me arrepenti</button>
            <button class="btn btn-light">Me Olvide algo</button>
            <button class="btn btn-success">Comproooo!</button>
        </div>
    </div>
</template>

<script>
export default {
    name:'CartDetail',
    props:{
        items:Array,
    }

}
</script>

<style scoped>
    .contenedorPrincipal{
    display: flex;
    flex-direction: column;
    row-gap: 10px;
    background-color: white;
    }
    .tituloCartContainer{
        width: 100%;
        padding: 10px;
        margin-top: 3%;
    }
    .tituloCart{
        text-align: center;
        font-family: 'Sriracha', cursive;
    }
    .datailCartContainer{
        padding: 7%;
    }
    .buttonCartContainter{
        display: flex;
        flex-direction: row;
        column-gap: 10px;
        align-items: center;
        justify-content: center;
        padding: 10px;
        margin-bottom: 3%;

    }

</style>