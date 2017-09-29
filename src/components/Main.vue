<template>
  <div class="main">
    <x-top></x-top>
    <x-content></x-content>
    <x-footer>
      <!--x-footer 에 html 등을 전달할때 slot 를 사용 -->
      <span slot="copyright">I-ON</span>
      <span slot="tel">02-3430-1200</span>
    </x-footer>
  </div>
</template>
<script>
  /* eslint-disable */
  import xTop from './X-Top.vue'
  import xContent from './X-Content.vue'
  import XFooter from "./X-Footer.vue";
  export default {
    components: {
      XFooter,
      'x-top': xTop,
      'x-content': xContent
    },
    name: 'main',
    data() {
      return {}
    }
  }
</script>
<style scoped>
  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }
</style>
