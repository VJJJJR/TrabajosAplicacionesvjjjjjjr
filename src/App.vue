<template>
    <h1 class="text-3xl font-bold underline">
  Hello world!
</h1>
<hr/>
<MyCounter :value="5"/>
<MyCountercopy :value="5"/>
<MyCountercopy3 :value="5"/>


    </template>

    <script lang="ts" setup>
import MyCounter from './Components/MyCounter.vue';
import MyCountercopy from './Components/MyCountercopy.vue';
import MyCountercopy3 from './Components/MyCountercopy.vue';


</script>
