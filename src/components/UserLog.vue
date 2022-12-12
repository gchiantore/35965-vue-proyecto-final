<template>
  <div class="container">
        <div class="row">
            <div class="logContainer col-md-12 col-lg-6">
                <div class="logTitulo">
                    <h1 class="textTitle">OK! vamo'a loguearnos</h1>
                </div>    
                <div class="logForm">
                    <form>
                        <div class="logInputs">
                            <div class="mb-3">
                                <label for="logEmail" class="form-label">Tu e-mail fiera!</label>
                                <input type="email" class="form-control" id="logEmail">
                            </div>
                            <div class="mb-3">
                                <label for="logPass" class="form-label">Tu clave ultra mega secreta</label>
                                <input type="password" class="form-control" id="logPass">
                            </div>
                        </div>
                        <div class="logButtons">
                            <button type="submit" class="btn btn-success">Atrodennnn</button>
                        </div>    
                    </form>
                </div>
                <div class="logRegistry">
                    <p>No tenes cuenta?, dont´t worry fiera, te hacemo'una al toque,<span>hace clic aqui!</span> </p>
                </div>    
            </div>
            <div class="imgContainer col-md-12 col-lg-6 d-none d-sm-none d-md-none d-lg-block">
                <img class="img-fluid" :src="require('@/assets/img/imglogin.png')" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
     name: 'UserLog',
}
</script>

<style scoped>
    .form-control:focus { 
    border-color: #28a745; 
    box-shadow: 0 0 0 0.2rem rgba(40, 167, 69, 0.25); 
    } 

    .textTitle{
        font-family: 'Sriracha', cursive;
        margin-bottom: 25px;
        margin-top: 30px;
        text-align: center;
    }

    .logContainer{
        display: flex;
        flex-direction: column;
        justify-content:space-between;
    }

    .logTitulo{
        padding: 15px;
        padding-top: 30px;
    }

    .logForm{
        padding: 15px;
    }

    .logRegistry{
        padding: 15px;
        margin-bottom: 20px;
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
        row-gap: 20px;
        padding: 5%;
    }
</style>
