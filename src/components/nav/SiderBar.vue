<template>
  <nav class="navbar navbar-default" id="nav-side">
      <ul class="nav nav-pills nav-stacked">
        <li><a href="#">01.准备</a></li>
        <li><a href="#">02.HelloWorld</a></li>
        <li><a href="#">03.Controller</a></li>
        <li><a href="#">04.View</a></li>
        <li><a href="#">05.Logic</a></li>
        <li><a href="#">06.异步处理</a></li>
        <li><a href="#">07.单元测试</a></li>
        <li><a href="#">08.文档生成</a></li>
        <li><a href="#">09.AOP应用</a></li>
      </ul>
  </nav>
</template>

<script>
export default {
  name: 'siderBar',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #nav-side {
    position: fixed;
    left: 0;
    top: 70px;
    width: 205px;
    height: 100%;
    background-color: #EBEBEB;
    font-size: 18px;
    text-align: left;
  }
  a {
    color: #546E7A;
  }
  li {
    padding: 0;
    margin: 0;
    border-bottom: 1px solid rgba(207,216,220,0.56);
  }
  .nav > li > a:hover, .nav > li > a:focus {
    background-color: #C2C2C2;
  }
</style>
