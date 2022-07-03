<template>
  <el-switch v-model="value1" />
  <el-switch
    v-model="value2"
    class="ml-2"
    style="--el-switch-on-color: #13ce66; --el-switch-off-color: #ff4949"
  />
   <types v-model:num="num"></types>
</template>

<script  setup>
import Types from '../components/Types.vue'
const value1 = ref(true)
const value2 = ref(true)

let num=ref(100)



</script>