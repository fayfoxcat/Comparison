<script lang="ts">
import {defineComponent} from 'vue'

export default defineComponent({
  name: "Target.vue"
})
</script>

<template>
  <div class="target-component">
    <!-- 组件的内容 -->
  </div>
</template>

<style scoped>
.target-component {
  width: 45%;
  height: 500px;
  border: 1px solid red;
  position: absolute;
  display: flex;
  right: 2.5%;
  top: 30px;
}
</style>