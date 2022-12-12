<template>
  <div id="app">
    <HelloWorld msg="Profecto Final 1ra Entrega - Guillermo Chiantore"/>
    <SeparadorComponentes titulo1="Formulario de Login" titulo2="UserLog.vue"></SeparadorComponentes>
    <UserLog></UserLog>
    <SeparadorComponentes titulo1="Formulario de Registro" titulo2="UserReg.vue"></SeparadorComponentes>
    <UserReg></UserReg>
    <SeparadorComponentes titulo1="Simulador de Carrito" titulo2="CartDetail.vue"></SeparadorComponentes>
    <CartDetail :items="carrito"></CartDetail>
    <SeparadorComponentes titulo1="Detalle de un Producto" titulo2="ProductDetail.vue"></SeparadorComponentes>
    <ProductDetail :product="products[0]"></ProductDetail>
    <SeparadorComponentes titulo1="Listado de Productos" titulo2="ProductList.vue contiene a CardProduct.vue"></SeparadorComponentes>
    <ProductList :productos="products"></ProductList>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import ProductDetail from './components/ProductDetail.vue'
import UserLog from './components/UserLog.vue'
import CartDetail from './components/CartDetail.vue'
import UserReg from './components/UserReg.vue'
import ProductList from './components/ProductList.vue'
import SeparadorComponentes from './components/SeparadorComponentes.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    ProductDetail,
    UserLog,
    CartDetail,
    UserReg,
    ProductList,
    SeparadorComponentes,
  },
  data(){
    return{
        products:[
            {
                id:"PMUSA01",
                img:"lamusa2.png",
                titulo:"La Mussa !",
                desc:"Si, e'la mas barata pero es potentaza",
                info1:"Masa crujiente como billetera a fin de mes, salada con autentica sal cordobeza de la Laguna Mar Chiquita, con tomates choriados de la quinta del tio Luis, y la mussa de la queseria de la suegra de Calamaro!",
                info2:"No podemos decir mas de este manjar solo para entendidos",
                info3:"Ideal pa'reponer hidratos y grasas perdidas en el picadito con los amigos, acompañada de una birrita helada pa'mantene la hidratacion!!",
                precio:1250,
            },
            {
                id:"PESPE01",
                img:"lamusa2.png",
                titulo:"La Especial !",
                desc:"Mamita que pizza!",
                info1:"Masa crujiente como billetera a fin de mes, salada con autentica sal cordobeza de la Laguna Mar Chiquita, con tomates choriados de la quinta del tio Luis, Jamon del Diome y la mussa de la queseria de la suegra de Calamaro!",
                info2:"Agregar mas seria una falta de respeto",
                info3:"Ideal pa'l domingo a la noche cuando llegas y tenes la heladera como para pintarla!",
                precio:1450,
            },
            {
                id:"PPALMI01",
                img:"lamusa2.png",
                titulo:"La Palmera!",
                desc:"Terrible Pizza!",
                info1:"Masa crujiente como billetera a fin de mes, salada con autentica sal cordobeza de la Laguna Mar Chiquita, con tomates choriados de la quinta del tio Luis, Jamon del diome, palmitos mas frescos que 1 de Julio y la mussa de la queseria de la suegra de Calamaro!",
                info2:"Cabe aclara que por cada mordiscoque le des nuestros proveedores plantan una plamera",
                info3:"Ideal pa'queda bien con la suegra y/o nuera, y si la acompañamos con un espumante ni te cuento",
                precio:1650,
            },
            {
                id:"PCHAM01",
                img:"lamusa2.png",
                titulo:"La Zetas! !",
                desc:"No puede mas, lo mejor de lo mejor",
                info1:"Masa crujiente como billetera a fin de mes, salada con autentica sal cordobeza de la Laguna Mar Chiquita, con tomates choriados de la quinta del tio Luis, con homgos extraido de la base del Champaqui durante los temporales de Junio y la mussa de la queseria de la suegra de Calamaro!",
                info2:"Si sguimo'hablando vamo'a ser spoilers",
                info3:"Ideal pa'cuando queres sorprender a tu pareja despues de haber hechado alto moco!, con un totin llegas al maridaje perfecto",
                precio:1850,
            },
         ],
         carrito:[
            {
              id:"PPALMI01",
              titulo:"La Palmera!",
              qty:1,
              pu:1650,
           },
           {
              id:"PESPE01",
              titulo:"La Especial !",
              qty:1,
              pu:1450,
           },
           {
              id:"PMUSA01",
              titulo:"La Mussa !",
              qty:1,
              pu:1250,
           },

        ],  
           
    }
  } 
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Sriracha&display=swap');
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.2/font/bootstrap-icons.css");
#app {
    font-family: 'Roboto Mono', monospace;
}

.form-control:focus { 
    border-color: #28a745; 
    box-shadow: 0 0 0 0.2rem rgba(40, 167, 69, 0.25); 
} 


</style>
