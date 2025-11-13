<template>
    <div class="home-container">
        <h1>Vue3教学</h1>
        <nav class="navigation">
            <router-link to="/new" class="nav-link">新组建集合</router-link>
        </nav>
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
        <stylebangding></stylebangding>
        <watchzhenting></watchzhenting>
        <biaodanshujubangding></biaodanshujubangding>
        <mobanyingyong></mobanyingyong>
        <zujianqiantao></zujianqiantao>
        <zujianchuanzhiprops></zujianchuanzhiprops>
        <propsjiaoyanA></propsjiaoyanA>
        <zujianshijian></zujianshijian>
        <zujianshijianVmodel></zujianshijianVmodel>
        <chaocaoslots></chaocaoslots>
        <shengmingzhouqi></shengmingzhouqi>
        <shengqingzhouyingyong></shengqingzhouyingyong>
        <dongtaizujian></dongtaizujian>
        <yibuzujian></yibuzujian>
        <yilaizhuruparent></yilaizhuruparent>
        <yilaizhuruchild></yilaizhuruchild>
        <yilaizhurusun></yilaizhurusun>
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
import stylebangding from '../components/stylebangding.vue';
import watchzhenting from '../components/watchzhenting.vue';
import biaodanshujubangding from '../components/biaodanshujubangding.vue';
import mobanyingyong from '../components/mobanyingyong.vue';
import zujianqiantao from '../components/zujianqiantao.vue';
import zujianchuanzhiprops from '../components/zujianchuanzhiprops.vue';
import propsjiaoyanA from '../components/propsjiaoyanA.vue';
import zujianshijian from '../components/zujianshijian.vue';
import zujianshijianVmodel from '../components/zujianshijianVmodel.vue';
import chaocaoslots from '../components/chaocaoslots.vue';
import shengmingzhouqi from '../components/shengmingzhouqi.vue';
import shengqingzhouyingyong from '../components/shengmingzhouqiyingyong.vue';
import dongtaizujian from '../components/dongtaizujian.vue';
import yibuzujian from '../components/yibuzujian.vue';
import yilaizhuruparent from '../components/yilaizhuruparent.vue';
import yilaizhuruchild from '../pages/yilaizhuruchild.vue';
import yilaizhurusun from '../pages/yilaizhurusun.vue';
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
        classbangding,
        stylebangding,
        watchzhenting,
        biaodanshujubangding,
        mobanyingyong,
        zujianqiantao,
        zujianchuanzhiprops,
        propsjiaoyanA,
        zujianshijian,
        zujianshijianVmodel,
        chaocaoslots,
        shengmingzhouqi,
        shengqingzhouyingyong,
        dongtaizujian,
        yibuzujian,
        yilaizhuruparent,
        yilaizhuruchild,
        yilaizhurusun,
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
.navigation {
    margin: 20px 0;
    z-index: 11;
}

.nav-link {
    display: inline-block;
    padding: 10px 20px;
    background-color: rgba(255, 255, 255, 0.1);
    color: white;
    text-decoration: none;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

.nav-link:hover {
    background-color: rgba(255, 255, 255, 0.3);
}
</style>