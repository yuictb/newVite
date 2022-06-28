<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <el-row class="mb-4">
    <el-button>Default</el-button>
    <el-button type="primary">Primary</el-button>
    <el-button type="success">Success</el-button>
    <el-button type="info">Info</el-button>
    <el-button type="warning">Warning</el-button>
    <el-button type="danger">Danger</el-button>
    <el-button>中文</el-button>
  </el-row>
  <div class="mb-2 flex items-center text-sm">
    <el-radio-group v-model="radio1" class="ml-4">
      <el-radio label="1" size="large">Option 1</el-radio>
      <el-radio label="2" size="large">Option 2</el-radio>
    </el-radio-group>
  </div>
  <div class="my-2 flex items-center text-sm">
    <el-radio-group v-model="radio2" class="ml-4">
      <el-radio label="1">Option 1</el-radio>
      <el-radio label="2">Option 2</el-radio>
    </el-radio-group>
  </div>
  <div class="my-4 flex items-center text-sm">
    <el-radio-group v-model="radio3" class="ml-4">
      <el-radio label="1" size="small">Option 1</el-radio>
      <el-radio label="2" size="small">Option 2</el-radio>
    </el-radio-group>
  </div>
  <div class="mb-2 flex items-center text-sm">
    <el-radio-group v-model="radio3" disabled class="ml-4">
      <el-radio label="1" size="small">Option 1</el-radio>
      <el-radio label="2" size="small">Option 2</el-radio>
    </el-radio-group>
  </div>
</template>
<script setup>
const radio1 = ref('1')
const radio2 = ref('1')
const radio3 = ref('1')
</script>
<style lang="less">
</style>
