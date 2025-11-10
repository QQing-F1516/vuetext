<template>
  <div>
    <h3>插槽总结</h3>
    <slot name="header"></slot>
    <a href="#">asdddddddddddddddddaaa</a>
    <slot name="content"></slot>
  </div>
</template>

<script>
export default {
  name: 'slotsxu',
  data() {
    return {
      // message: 'slotsxu'
    }
  }
}
</script>