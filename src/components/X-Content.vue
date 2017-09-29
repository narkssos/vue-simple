<template>
  <div class="content">
    <h4>여기는 그냥 HTML</h4>
    <div>{{msg}}</div>
  </div>
</template>

<script>
  /* eslint-disable */
export default {
  name: 'content',
  data () {
    return {
      msg: '이건 데이터 메세지'
    }
  }
}
</script>
<style scoped>
.content{
  border:1px solid #cecece;
  padding:25px;
  margin:20px 40px;
}
</style>
