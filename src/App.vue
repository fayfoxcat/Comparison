<script setup lang="ts">
</script>

<template>
  <div class="max_box">
<!--    <Input/>-->
<!--    <Result/>-->
  </div>

</template>

<script>

import Input from '@/components/Input.vue'
import Result from '@/components/Result.vue'

export default {
  name: 'App',
  components: {
    Input, Result
  },
  // 在这里可以使用选项式API定义数据、方法等
}
</script>

<style scoped>
.max_box {
  width: 180vh;
  height:500px;
  margin: 0;
  border: 1px solid black;
}
</style>
