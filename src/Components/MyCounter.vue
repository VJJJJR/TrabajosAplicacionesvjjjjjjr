<template>
    <h1>hola mundo</h1>
<h3>Contador: {{contador}}</h3>
<h3>Cuadrado: {{ contador*contador}}</h3>

<div>
<button v-on:click="contador++">+1</button>
<button v-on:click="contador--">-1</button>

</div>

    </template>

    <script lang="ts" setup>



    import {ref} from 'vue';
    
console.log("hola mundo");
const props = defineProps<{
value: number;


}>();
const contador= ref(props.value);
</script>
<style scoped>
h1{color: red;


}

</style>