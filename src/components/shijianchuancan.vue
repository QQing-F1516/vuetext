<template>
    <div class="shijianchuancan">
        <hr>
        <h3>事件传参</h3>
        <!-- 1.默认参数 -->
        <button  class="count1"  @click="count1">add 123</button>
        <p>count is {{ countNum }}</p>
        <!-- 2.-->
         <button class="newcount" @click="newcount">newcount 123</button>
         <hr>
    </div>
</template>

<script>
export default {
    name: 'shijianchuancan',
    data() {
        return {
            countNum: 0,
            newcount: 20
        }
    },
    methods: {
        count1(e) {
            console.log(e,'count1');
            console.log(e.target,'e.target');
            console.log(e.currentTarget,'e.currentTarget');
            console.log(e.target.innerHTML,'e.target.innerHTML');
            e.target.innerHTML = 'tianjia添加' + this.countNum;
            this.countNum += 123;
        },
        newcount(msg) {
            console.log(msg,'newcount');
        }
    }
}

</script>

<style>
.shijianchuancan{
    color: royalblue;
    font-size: 35px;
}
.count1{
    font-size: 25px;
}
.newcount{
    font-size: 25px;
}
</style>