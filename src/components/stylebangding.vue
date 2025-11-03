<template>
    <div class="stylebangding">
        <h3>样式绑定</h3>
        <p :style="{color: activeColor, fontSize: fontSizeNum +'px'}">
            1.行内样式绑定
        </p>
        <p :style="ObjecStyle">
            2.行内样式绑定-对象语法
        </p>
    </div>
</template>

<script>
export default {
    name: 'stylebangding',
    data() {
        return {
            activeColor: 'red',
            fontSizeNum: 30,
            ObjecStyle: {
                color: 'blue',
                fontSize: '30px'
            }
        }
    }
}
</script>

<style>
.stylebangding {
    color: green
}
</style>