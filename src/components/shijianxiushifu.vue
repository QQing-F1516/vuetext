<template>
    <div class="shijianxiushifu">
        <h3>事件修饰符</h3>
        <!-- <a @click="click11" href="http://www.baidu.com">百度</a> -->
        <!-- 阻止事件默认行为 -->
        <a @click.prevent="click11" href="http://www.baidu.com">百度</a>
        <!-- 阻止事件冒泡 -->
         <div @click="clickDiv">
            <p @click.stop="clickp">测试冒泡</p> <!-- 在后面加.stop -->
         </div>
         <hr>
    </div>
</template>

<script>
export default {
    name: 'shijianxiushifu',

    data(){
        return{

        }
    },
    methods:{
        click11(e){
            // e.preventDefault();//1.阻止默认跳转
            console.log('点击了百度');
        },
        clickDiv() {
            console.log('点击了div');
        },
        clickp() {
            console.log('点击了p');
        },
    },

}
</script>

<style>
.shijianxiushifu{
    color: slateblue;
}
</style>