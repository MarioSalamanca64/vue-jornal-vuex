<template lang="">
<div class="entry-title d-flex justify-content-between p-2">
    <div>
        <span class="text-success fs-3 fw-bold">15</span>
        <span class="mx-1 fs-3">Julio</span>
        <span class="mx-2 fs-4 fw-light">2021, jueves</span>
    </div>

    <div>
        <button class="btn btn-danger mx-2">
            Borrar
            <i class="fas fa-trash-alt"></i>
        </button>
        <button class="btn btn-primary">
            Subir foto
            <i class="fas fa-upload"></i>
        </button>
    </div>
</div>

 <hr>
<!-- vue 3 solamente -->
<div class="d-flex flex-column px-3 h-75">
    <textarea
    placeholder="¿Que sucesio hoy?">
    </textarea>
</div>

<Fab
    icon="fa-save"
/>

<img src="https://media.istockphoto.com/id/1296165226/es/foto/campo-de-soja-abierto-al-atardecer-campo-de-soja.jpg?s=1024x1024&w=is&k=20&c=sACFf_oXo-rMlyxXEBLkm5WxaCjQmP6sQ7WABn91lHc=" 
     alt="entry-picture"
     class="img-thumbnail">

</template>
<script>
import { defineAsyncComponent } from 'vue';

export default {
    components:{
        Fab: defineAsyncComponent(() => import('../components/Fab-component.vue'))
    }
}
</script>

<style lang="scss" scoped>
    textarea{
        font-size:20px;
        border:none;
        height:100%;

        &:focus{
            outline: none;
        }
    }
    img{
        width: 200px;
        position: fixed;
        bottom: 150px;
        right: 20px;
        box-shadow: 0px 5px 10px rgba($color:#0000, $alpha:0.2);
    }
</style>