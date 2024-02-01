<script setup lang="ts">
</script>

<template>
  <div class="max_box">
    <Input/>
    <Result/>
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
  position: absolute;
  width: 100%;
  height:1100px;
  display: flex;
  flex-wrap: wrap;
  align-content: space-between;
  border: 1px solid blue;
  margin-top: 0;
  margin-right: 0;
}
</style>
