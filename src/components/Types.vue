<template>
    <div>这是一个子组件</div>
    <button @click="change">{{num}}</button>
</template>

<script setup>
const props= defineProps({
    num: {
        type: Number,
        defalult: 100
    }
})
const emit=defineEmits(['update:num'])
const change=()=>{
    emit('update:num',500)
}
console.log(props.num)
</script>