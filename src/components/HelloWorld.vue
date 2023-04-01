<script setup lang='ts'>
const inputVal = ref('test')
</script>

<template>
<div class="main-container">
  <a-input type="text" v-model:value="inputVal" />
  <span>{{ inputVal }}</span>
</div>
</template>

<style lang='less' scoped>
.main-container {
  display: flex;
  flex-direction: column;
  font-size: 32px;

  &>input {
    font-size: 32px;
    text-align: center;
  }

  &>span {
    margin-top: 20px;
  }
}
</style>