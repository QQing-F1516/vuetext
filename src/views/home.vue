<template>
    <div class="home-container">
        <h1>Vue3教学</h1>
        <hr>
        <Mobanyufa></Mobanyufa>
        <Shuxingbangding></Shuxingbangding>
        <tiaojianxuanran></tiaojianxuanran>
    </div>
</template>


<script>
import Mobanyufa from '../components/mobanyufa.vue'
import Shuxingbangding from '../components/shuxingbangding.vue' 
import tiaojianxuanran from '../components/tiaojianxuanran.vue';    

export default {
    name: 'home',
    components: {
        Mobanyufa,
        Shuxingbangding,
        tiaojianxuanran
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