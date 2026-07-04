<script setup>
import {ref} from 'vue'
const username = ref('')
</script>
<template>
<input type="text" v-model="username" placeholder="Введи свое имя">
</input>
<h1 v-show="username">Привет {{username}}!</h1>
</template>
