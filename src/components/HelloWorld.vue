<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <button @click="change">按钮</button>
  </div>
</template>
<script setup>
let vvs=ref(158366565)
defineProps({
  msg: {
    type: String,
    default: 'ijiii'
  }
})
const emit=defineEmits(['fn'])
const change=()=>{
  emit('fn',vvs)
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
