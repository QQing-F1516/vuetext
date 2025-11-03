<template>
    <div class="mobanyingyong">
        <h3>模板引用</h3>
        <div class="container" ref="container">
            {{ content }}
        </div>
        <button @click="changeContent">改变内容</button>
        <br>
        <input type="text" ref="username"></input>
    </div>
</template>

<script>
export default {
    name: 'mobanyingyong',
    data() {
        return{
            content: '模板引用'
        }
    },
    methods: {
        changeContent() {
            console.log(this.$refs.container,"1221212121");
            this.$refs.container.innerHTML = "565656";
            console.log(this.$refs.username,"1221212121");
        }
    }
}
</script>

<style>
.mobanyingyong {
    color: yellow;
}
</style>