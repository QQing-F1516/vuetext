<template>
    <div class="jisuanshuxing">
        <h3>计算属性</h3>
        <p>{{ content.name }}</p>
        <div>{{ content.text.length > 2 ? "yes" : "no"}}</div>
        <div>{{ content.results.length > 0 ? (content.text1.length > 0 ? "yes" : "55555") : "222222" }}</div>
        <p>{{ isResults }}</p>
        <p>{{ isDatat() }}</p>
        <hr>
    </div>  
</template>

<script>
export default {
    name: 'jisuanshuxing',
    data() {
        return {
            content: {
                name : 'qq',
                text: ["1", "2", "3", "4", "5"],
                arr:[{name:"11", id:1},{name:"22", id:2}],
                results:[
                {
                    "gkey": "102094960",
                    "qcmsint1": "0",
                    "w64": -1,
                    "gtype": "3",
                    "title": "双人游戏大全",
                    "url": "http://360game.360.cn/flash/102094960.html",
                    "gdata": "{\"type\":\"flashgame\",\"appid\":\"102094960\"}",
                    "name": "双人游戏大全",
                    "img": "//p0.qhimg.com/d/appstorage/74fcbb1da492f34b5ba49d99549afba0.png"
                },
                {
                    "gkey": "102144745",
                    "qcmsint1": "0",
                    "w64": -1,
                    "gtype": "3",
                    "title": "餐厅游戏大全",
                    "url": "http://360game.360.cn/flash/102144745.html",
                    "gdata": "{\"type\":\"flashgame\",\"appid\":\"102144745\"}",
                    "name": "餐厅游戏大全",
                    "img": "//p2.qhimg.com/t01c4a2f17a198def57.png"
                },
                {
                    "gkey": "102144642",
                    "qcmsint1": "0",
                    "w64": -1,
                    "gtype": "3",
                    "title": "火柴人游戏合集",
                    "url": "http://360game.360.cn/flash/102144642.html",
                    "gdata": "{\"type\":\"flashgame\",\"appid\":\"102144642\"}",
                    "name": "火柴人游戏合集",
                    "img": "//p1.qhimg.com/t0147f6ec029fefe8d7.png"
                }
                ],
                text1: []
            }
        };
    },
    computed: {
        isResults() {

            return this.content.results.length > 0 ? (this.content.text1.length > 0 ? "yes" : "1111111") : "222222";

        }
    },
    methods: {
        isDatat() {
            return this.content.results.length > 0 ? (this.content.text1.length > 0 ? "yes" : "66666666") : "222222";
        }
    }
}
</script>

<style>
.jisuanshuxing{
    color: red;
}
</style>