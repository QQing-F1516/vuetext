<template>
    <div class="zuheshijianchuli">
        <hr>
        <h3>组合式---事件处理</h3>
        <p>{{ count }}</p>
        <button @click="addCount">增加</button>
        
        <hr>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)

function addCount() {
    console.log('点击了', '--------');
    count.value++;
}
</script>

<style scoped>
.zuheshijianchuli {
    color: pink;
}
</style>