
<template>
  <div class="input-component">
    <!-- 组件的内容 -->
  </div>
</template>

<script lang="ts">
import {defineComponent} from 'vue'
import Original from './Original.vue'
import Target from './Target.vue'

export default defineComponent({
  name: "Input.vue",
  components: {
    Original,Target
  },
})

</script>

<style scoped>
.input-component {
  width: 1024px;
  height: 500px;
  border: 1px solid goldenrod;
}
</style>