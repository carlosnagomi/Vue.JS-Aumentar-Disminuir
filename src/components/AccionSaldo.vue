<template>
  <button @click="accion()" :disabled="desactivar"> {{ texto }}</button>
</template>

<script>
export default {
    name:'AccionSaldo',
    props:{
        texto: String,
        desactivar: {
           type: Boolean,
           default: false
        } 
    },
    methods:{
        accion(){
            this.$emit('accion')
        }
    },
    data() {
        return {
            
        }
    },
}
</script>

<style>

</style>