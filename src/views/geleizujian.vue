<template>
  <div class="divdiv" v-if="showContent">
    <h3 class="title">分类组件+++++</h3>
    <nav class="navigation">
      <router-link to="/new" class="nav-link">跳转到new</router-link>
    </nav>
    <hr>
    <swiper></swiper>
    <hr>
  </div>
</template>

<script>

import swiper from "../nnewcomponents/swiper.vue"

export default {
  name: 'geleizujian',
  data() {
    return {
      showContent: false,
    }
  },
  components: {
    swiper
  },

  mounted() {
    setTimeout(() => {
      this.showContent = true;
    }, 0);
  }
}
</script>

<style scoped>
.divdiv {
  position: relative;
  z-index: 11;
}

.title {
  color: red;
  margin-bottom: 20px;
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