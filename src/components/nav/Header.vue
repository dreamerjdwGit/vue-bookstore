<template>
  <nav class="navbar navbar-default  navbar-fixed-top" role="navigation">
      <div class="navbar-header">
        <a class="navbar-brand" href="#"><span>hifive</span></a>
      </div>
      <ul class="nav nav-pills" id="main-nav" @click="select()">
        <li data-id="1"><a href="#">自习篇</a></li>
        <li><a href="#">基本篇</a></li>
        <li><a href="#">数据模型篇</a></li>
        <li><a href="#">数据绑定篇</a></li>
      </ul>
  </nav>
</template>

<script>
export default {
  name: 'header',
  methods: {
    select: function() {
      var target = event.currentTarget;
      alert(target.tagName)
      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .navbar {
    width:100%;
    height: 70px;
    background: #6B8E23;
  }
  .navbar span {
    display: none;
  }
  .navbar-header {
    float: left;
    width: 205px;
    height: 100%;
    background: url('../../../static/img/icon_hifiveLogo.png') no-repeat;
  }
  a:visited {
    background-color: #458B00 !important;
  }
  .nav > li > a {
    height: 68px;
    width: 140px;
    line-height: 55px;
    font-size: 20px;
    text-align: center;
    background: transparent;
    color: #fff;
  }
  .nav > li.active > a:hover{
    background-color: #458B00;
  }
  .nav > li.active > a{
    background-color: #458B00;
  }
</style>
