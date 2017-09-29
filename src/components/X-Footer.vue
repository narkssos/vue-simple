<template>
  <div class="x-footer">
    <div>
      <slot name="copyright"></slot>
      <slot name="tel"></slot>
    </div>
  </div>
</template>
<script>
  /* eslint-disable */
  import $ from 'jquery'

  export default {
    name: 'x-footer',
    data() {
      return {}
    },
    methods: {

    }
  }
</script>
<style scoped>
  .x-footer >  *{
    font-size:12px;
  }
</style>
