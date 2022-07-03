<template>
  <div class="home">
    {{num}} ==== {{is}}
    <HelloWorld @fn="fhu" :msg="ismsg" />
  </div>
</template>

<script setup>
import {useStore} from '../store'
import HelloWorld from "../components/HelloWorld.vue";
const store=useStore()
const {num}=storeToRefs(store)
let ismsg=ref('欢迎使用vue3.0...........');
let is=ref('初始')
const fhu=(n)=>{
  is.value=n;
  num.value=n
}
</script>
