<script setup lang="ts">
import {defineComponent} from 'vue'

import {UploadFilled} from '@element-plus/icons-vue'
import * as XLSX from "xlsx";

defineComponent({
  name: "Original.vue"
})


function handleBeforeUpload(file: File) {
  const reader = new FileReader();

  reader.onload = (e: ProgressEvent<FileReader>) => {
    if (e.target) {
      const arrayBuffer = e.target.result as ArrayBuffer;
      const data = new Uint8Array(arrayBuffer);
      const workbook = XLSX.read(data, {type: 'array'});

      const firstSheetName = workbook.SheetNames[0];
      const worksheet = workbook.Sheets[firstSheetName];

      const json = XLSX.utils.sheet_to_json(worksheet);
      console.log(json);
    } else {
      console.error('FileReader event target is null.');
    }
  };

  reader.readAsArrayBuffer(file);
  return false;
}

</script>

<template>
  <div class="original-component">
    <el-upload
        class="upload-demo"
        drag
        action="#"
        :before-upload="handleBeforeUpload"
        multiple
        accept=".xlsx, .xls"
    >
      <el-icon class="el-icon--upload">
        <upload-filled/>
      </el-icon>
      <div class="el-upload__text">
        将文件拖放到此处或<em>点击上传</em>
      </div>
      <template #tip>
        <div class="el-upload__tip">
          大小小于500kb的jpg/png文件
        </div>
      </template>
    </el-upload>
  </div>
</template>

<style scoped>
.original-component {
  width: 45%;
  height: 430px;
  border: 1px solid red;
  position: absolute;;
  display: flex;
  left: 2.5%;
  top: 30px;
}
</style>