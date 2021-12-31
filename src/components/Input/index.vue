<!--
 * @Author: your name
 * @Date: 2021-12-31 15:08:19
 * @LastEditTime: 2021-12-31 15:26:18
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: /input-project/src/components/HelloWorld.vue
-->
<script setup>
defineProps({
  placeholder: {
    type: String,
    default: () => "",
  },
  disabled: {
    type: Boolean,
    default: () => false,
  },
  width: {
    type: Number,
    default: () => 220,
  },
  height: {
    type: Number,
    default: () => 36,
  },
  value: {
    type: String,
    default: () => "",
  },
  name: {
    type: String,
    default: () => "",
  },
});
</script>

<template>
  <input
    :style="{ width: `${width}px`, height: `${height}px` }"
    type="text"
    :name="name"
    v-model="value"
    :placeholder="placeholder"
    :disabled="disabled"
  />
</template>

<style scoped>
input {
  border: 1px solid #ccc;
  border-radius: 5px;
  outline: 0;
}
</style>
