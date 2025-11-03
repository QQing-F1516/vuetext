<template>
    <div class="biaodanshujubangding">
        <hr>
        <h2>表单数据绑定</h2>
        <form>
            <input type="text" v-model.lazy="lazya"></input>
            <p>{{ lazya }}</p>
            <p>Message is : {{ message }}</p>
            <input type="checkbox" id="checkbox" v-model="checked"></input>
            <label for="checkbox">{{ checked }}</label>
        </form>
    </div>
</template>

<script>
export default {
    name: 'biaodanshujubangding',
    data() {
        return {
            lazya: '2223324242',
            message: 'Hello Vue!',
            checked: true
        }
    }
}
</script>

<style>
.biaodanshujubangding {
    color: white;
}
</style>