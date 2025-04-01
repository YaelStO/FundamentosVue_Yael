<template>
    <div class="container">
        <div class="row mt-4">
            <button @click="clic" class="btn btn-danger" type="button"> Dale Clic</button>
            <button @click="soyBoton" class="btn btn-warning mx-2" type="button"> Dale Clic 2</button>
            
        </div>
        <div>
            <!--h4>Evento Change</!--h4>
            <label class="input-group-text" for="">Ingresa tu nombre</label>
            <input class="form-control mt-2" type="text" id="nombre" @change="nombreE"-->
        </div>
    </div>
</template>
<script>
export default {
    methods:{
        clic(){
            alert("Gracias por darle clic")
        },
        soyBoton(){
            alert("soy un boton")

        }
    }
}
</script>
<style>
    
</style>