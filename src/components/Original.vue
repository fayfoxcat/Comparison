<script lang="ts">
import {defineComponent} from 'vue'

export default defineComponent({
  name: "Original.vue"
})
</script>

<template>
  <div class="original-component">
    <!-- 组件的内容 -->
  </div>
</template>

<style scoped>
.original-component {
  width: 45%;
  height: 500px;
  border: 1px solid red;
  position: absolute;
  display: flex;
  left: 2.5%;
  top: 30px;
}
</style>