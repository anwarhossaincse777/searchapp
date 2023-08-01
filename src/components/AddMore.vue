
<script setup>
import {ref} from "vue";

const favColors = ref([''])

function addColour(){
favColors.value.push('')

}

</script>



<template>
  <section class="mx-auto container">
    <h1 class="text-2xl mb-10">Color of the click</h1>
    <p class="mb-10">{{ favColors }}</p>
    Your favorite colors <br/>
    <div class="flex flex-col">
      <input class=" m-2" type="text" v-model="favColors[n-1]" v-for="(n,index) in favColors.length" :key="index">
    </div>
    <button @click="addColour()">Add More Colour</button>
  </section>
</template>



<style scoped>

</style>