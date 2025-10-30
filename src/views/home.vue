<template>
    <div class="home-container">
        <h1>Vue3教学</h1>
        <hr>
        <Mobanyufa></Mobanyufa>
        <Shuxingbangding></Shuxingbangding>
        <tiaojianxuanran></tiaojianxuanran>
        <liebiaoxuanran></liebiaoxuanran>
        <keyguanlizhuangtai></keyguanlizhuangtai>
        <shijianchuli></shijianchuli>
        <shijianchuancan></shijianchuancan>
        <shijianxiushifu></shijianxiushifu>
        <shuzubianhuazhence></shuzubianhuazhence>
        <jisuanshuxing></jisuanshuxing>
        <classbangding></classbangding>
    </div>
</template>


<script>
import Mobanyufa from '../components/mobanyufa.vue'
import Shuxingbangding from '../components/shuxingbangding.vue' 
import tiaojianxuanran from '../components/tiaojianxuanran.vue';    
import liebiaoxuanran from '../components/liebiaoxuanran.vue';
import keyguanlizhuangtai from '../components/keyguanlizhuangtai.vue';
import shijianchuli from '../components/shijianchuli.vue';
import shijianchuancan from '../components/shijianchuancan.vue';
import shijianxiushifu from '../components/shijianxiushifu.vue';
import shuzubianhuazhence from '../components/shuzubianhuazhence.vue';
import jisuanshuxing from '../components/jisuanshuxing.vue';
import classbangding from '../components/classbangding.vue';
export default {
    name: 'home',
    components: {
        Mobanyufa,
        Shuxingbangding,
        tiaojianxuanran,
        liebiaoxuanran,
        keyguanlizhuangtai,
        shijianchuli,
        shijianchuancan,
        shijianxiushifu,
        shuzubianhuazhence,
        jisuanshuxing,
        classbangding
    },
}
</script>

<style scoped>
.home-container {
    position: relative;
    z-index: 10;
}

h1 {
    z-index: 11;
    color: aqua;
}

</style>