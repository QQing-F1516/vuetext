<template>
    <div class="watchzhenting">
        <hr>
        <h3>watch侦听</h3>
        <p>
            {{message}}
        </p>
        <button @click="update">修改数据</button>
    </div>
</template>

<script>
export default {
    name: 'watchzhenting',
    data() {
        return {
            message:'watchzhenting'
        }
    },
    methods: {
        update() {
            this.message = '1122111222';
        }
    },
    watch: {
        message(newValue,oldValue) {
            console.log(newVal,'11111111111111');
            console.log(oldValue,'222222222222222');
        }
    }
}
</script>

<style>
.watchzhenting {
    color: blueviolet;
}
</style>