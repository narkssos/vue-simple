<template>
  <div class="x-top">
    <ul>
      <li v-for="item in items" @click="click">{{item.text}}</li>
    </ul>
  </div>
</template>
<script>
  /* eslint-disable */
  import $ from 'jquery'

  export default {
    name: 'x-top',
    data() {
      return {
        items: [
          {text: 'MENU1'},
          {text: 'MENU2'},
          {text: 'MENU3'},
          {text: 'MENU4'}
        ]
      }
    },
    methods: {
      click: function (e) {
        console.log('click', $(e.target).text())
      }
    }
  }
</script>
<style scoped>
  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    cursor: pointer;
    display: inline-block;
    margin: 0 10px;
  }
</style>
