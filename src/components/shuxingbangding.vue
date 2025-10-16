<template>
    <div class="shuxingbangding">
        <hr>
        <h3>属性绑定</h3>
        <p :id="dynamicId" :class="dynamicClass" :title="titleaaa" :aaa="aaa">测试</p>
        <button :disabled="isButtonDisabled">按钮</button>
        <div v-bind="obiectOFAttrs">三亚学院</div>
    </div>
</template>

<script>
export default {
  name: 'shuxingbangding',

  data() {
    return {
        dynamicId:'id1',
        dynamicClass:'class1',
        titleaaa:'title1',
        isButtonDisabled:true,
        aaa:undefined,
        obiectOFAttrs:{
            id:'id2',
            class:'class2',
        }
    }
  },
}
</script>

<style>
.shuxingbangding{
    color: white;
    
}
#id1{
    color: red;
}
.class1{
    font-size: 50px;
}
.class2{
    color: blue;
}
#id2{
    font-size: 80px;
}
</style>