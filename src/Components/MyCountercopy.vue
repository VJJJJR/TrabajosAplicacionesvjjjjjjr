<template>
    <h1>hola mundo</h1>
<h3>Contador: {{contador}}</h3>
<h3>Cuadrado: {{ contador*contador}}</h3>

<div>
<button v-on:click="contador++">+1</button>
<button v-on:click="contador--">-1</button>

</div>

    </template>

    <script lang="ts" >
    import { defineComponent, ref } from 'vue';
export default defineComponent({
    props:{
        value:{type:Number, required:true}
    },

    setup(props) {
        
const contador=ref(props.value);
return {contador: contador}

    },
})

</script>
<style scoped>
h1{color: red;


}

</style>