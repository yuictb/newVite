<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button @click="change">{{num}}</button>
      {{a}}    {{b}}   {{comput}}
  </div>
</template>
<script setup>
  let num=ref(0)
  let obj=reactive({
      a:1,
      b:2,
      c:3
  })
  let {a,b,c}=toRefs(obj)
  const change=()=>{
    comput.value=11124
      console.log(comput.value)
  }
  let comput=computed({
    get(){
        return a=789
    },
    set(value){
       console.log('变化')
    }
  })
</script>
<style lang="less"></style>
