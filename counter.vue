<script setup>
import {ref} from 'vue'


const counter = ref(0)
function increment(){
  counter.value++
}

function decrement() {
  if (counter.value > 0) {
    counter.value--
  }
}

function reset() {
  counter.value = 0
}

</script>

<template>
  <h1>Счетчик: {{counter}}</h1>
  <button id="up" @click="increment">Увеличить</button>
  <button id="down" @click="decrement">Уменьшить</button>
  <button id="reset" @click="reset">Сбросить</button>
</template>

<style scoped>
#up, #down, #reset {
  color: red;
  font-size: 40px;
  width: 300px;
  height: 50px;
}
#reset {
  margin-top: 5%;
  margin-left: 25%;
}
</style>