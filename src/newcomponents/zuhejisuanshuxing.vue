<template>
  <div class="zujijuanshuxing">
    <hr>
    <h3>组合式API---计算属性</h3>
    <p>{{ message }}</p>
    <p>{{ userInfo.name }}</p>
    <p>{{ reverserMessage }}</p>
    <p>{{ reverserUserInfoName }}</p>
    <p>{{ demo }}</p>
  </div>
</template>

<script setup>
import { ref, reactive, computed } from 'vue';
import { myDemo } from '../utils/computedUtils';

const message = ref("abcdasdf");
const userInfo = reactive({
  name: "张三",
  age: 18,
  sex: "男"
});

 
const reverserMessage = computed(() => {
  // [script] 必须通过 .value才能读到值
  return message.value.split("").reverse().join("");
});

 
const reverserUserInfoName = computed(() => {
  return userInfo.name.split("").reverse().join("");
});

const demo = myDemo(message);
</script>

<style scoped>
.zujijuanshuxing {
  color: red;
}
</style>