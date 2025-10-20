<template>
    <div class="shijianchuli">
        <hr>
        <h3>事件处理</h3>
        <button @click="count++">ADD 1</button>
        <p>Count is : {{ count }}</p>
        <!-- 通常必须使用以下方法处理器 -->
        <h4>方法事件处理器</h4>
        <button @click="addCount()">ADD 2</button>
        <p>isis : {{ countNum }}</p>
    </div>
</template>

<script>
export default {
    name: 'shijianchuli',
    data() {
        return {
            count: 0,
            countNum: 0
        }
    },
    methods: {
        addCount() {
            this.countNum += 2;
        }
    }
}
</script>

<style>
.shijianchuli{
    color: yellow;
}
</style>