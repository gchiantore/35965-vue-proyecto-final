<template>
  <div class="container">
        <div class="row">
            <div class="logContainer col-md-12 col-lg-6">
                <div class="logTitulo">
                    <h1 class="textTitle">Te vamo'a pedir info OK??</h1>
                </div>    
                <div class="logForm">
                    <form>
                        <div class="logInputs">
                            <div class="mb-3">
                                <label for="nombre" class="form-label">Como te llamas ?</label>
                                <input type="text" class="form-control" id="nombre">
                            </div>
                            <div class="mb-3">
                                <label for="direccion" class="form-label">Donde Vivis? (Calle, numero, barrio, ciudad)</label>
                                <input type="text" class="form-control" id="direccion">
                            </div>
                            <div class="mb-3">
                                <label for="nac" class="form-label">Cuando Naciste? Capas pa'l cumple te mandamo'algo</label>
                                <input type="date" class="form-control" id="nac">
                            </div>
                            <div class="mb-3">
                                <label for="regEmail" class="form-label">Tu mail??</label>
                                <input type="email" class="form-control" id="regEmail">
                            </div>
                            <div class="mb-3">
                                <label for="regPass" class="form-label">Pone una clave ultre mega secreta!</label>
                                <input type="password" class="form-control" id="regPass">
                            </div>
                        </div>
                        <div class="logButtons">
                            <button type="submit" class="btn btn-success">Listortiii</button>
                        </div>    
                    </form>
                </div>
                <div class="logRegistry">
                    <p class="text-center">Ya tenes cuenta?? que hace' aca!??  <span>Vamo' a loguearnos! </span> </p>
                </div>    
            </div>
            <div class="imgContainer col-md-12 col-lg-6 d-none d-sm-none d-md-none d-lg-block">
                <img class="img-fluid" :src="require('@/assets/img/imgregistro.png')" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'UserReg'
}
</script>

<style scoped>
    form-control:focus { 
    border-color: #28a745; 
    box-shadow: 0 0 0 0.2rem rgba(40, 167, 69, 0.25); 
    } 

    .textTitle{
        font-family: 'Sriracha', cursive;
        margin-bottom: 25px;
        margin-top: 10px;
        text-align: center;
    }

    .logContainer{
        display: flex;
        flex-direction: column;
        justify-content:space-between;
    }

    .logTitulo{
        padding: 5px;
        padding-top: 5px;
    }

    .logForm{
        padding: 5px;
    }

    .logRegistry{
        padding: 10px;
        margin-bottom: 5px;
    }

    .logInputs{
        display: flex;
        flex-direction: column;
        row-gap: 20px;
        padding: 5%;
    }

    .logButtons{
        display: flex;
        flex-direction: column;
        padding: 5%;
    }
</style>