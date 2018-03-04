<template>
  <div class="container">
    <x-header>VUX</x-header>
    <div class="remain">{{msg}}</div>
  </div>
</template>

<script>
  import {XHeader} from 'vux'

  export default {
    name: 'HelloWorld',
    data() {
      return {
        msg: '欢迎使用vuxwebpack!'
      }
    },
    components: {
      XHeader,
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
  .container{
    display: flex;
    flex-direction: column;
    height: 100vh;
    & .remain{
      flex: 1;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 0 20px;
    }
  }

</style>
