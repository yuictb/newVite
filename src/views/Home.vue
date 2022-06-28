<template>
  <div class="home">
    <img @click="changenum" alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld :msg="ismsg" />
  </div>
</template>

<script setup>
import {useStore} from '../store'
// import { storeToRefs } from 'pinia';
import HelloWorld from "../components/HelloWorld.vue";
const store=useStore()
const {num}=storeToRefs(store)
console.log(store.num)
const changenum=()=>{
   num.value=50000
}
let ismsg=ref('欢迎使用vue3.0');
</script>
