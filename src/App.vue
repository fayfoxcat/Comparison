<script setup lang="ts">
</script>

<template>
  <Original/>
  <Target/>
  <Result/>

</template>

<script>
import Original from './components/Original.vue'
import Target from './components/Target.vue'
import Result from './components/Result.vue'

export default {
  name: 'App',
  components: {
    Original, Target,Result
  },
  // 在这里可以使用选项式API定义数据、方法等
}
</script>

<style scoped>

</style>
