<template>
  <div>插槽测试</div>
  <slot name="header" :msg="childMsg"></slot>
  <slot name="main" :job="jobMsg"></slot>
</template>

<script>
export default {
  name: "slotzaxu",
  data() {
    return {
      childMsg: "这小子娇羞西",
      jobMsg: "反对反对反对"
    }
  }
}
</script>