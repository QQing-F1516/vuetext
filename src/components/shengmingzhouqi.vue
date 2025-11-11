<template>
  <div class="shengqingzhouyi">
    <hr>
    <h1> 这是生命周期</h1>
    <p v-if="msg">{{msg}}</p>
    <button @click="updateMsg">更新数据</button>
  </div>
</template>

<script>
// 生命周期：
// 挂载前：beforeCreate created
// 挂载中：beforeMount mounted
// 更新前：beforeUpdate updated
// 卸载前：beforeUnmount unmounted

export default {
  name: 'shengqingzhouyi',
  data() {
    return {
      msg: '盛情之辉'
    }
  },
  methods: {
    updateMsg() {
      this.msg = '更新之辉';
    }
  },
  beforeCreate() {
    console.log('盛情之辉');
  },
  created() {
    console.log('盛情之辉');
  },
  beforeMount() {
    console.log('盛情之辉');
  },
  mounted() {
    console.log('盛情之辉');
  },
  beforeUpdate() {
    console.log('盛情之辉');
  },
  updated() {
    console.log('盛情之辉');
  },
  beforeUnmount() {
    console.log('盛情之辉');
  },
  unmounted() {
    console.log('盛情之辉');
  }
}
</script>

<style scoped>
.shengqingzhouyi {
  color: aqua;
}
</style>