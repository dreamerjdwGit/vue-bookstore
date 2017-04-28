<template>
  <div class="container" id="wrapper">
    <book-header-nav></book-header-nav>
    <book-side-nav></book-side-nav>
    <div class="main">
      <book-content></book-content>
    </div>
    <book-footer></book-footer>
  </div>
</template>

<script>
import bookHeader from './components/nav/Header'
import bookSider from './components/nav/SiderBar'
import bookFooter from './components/footer/Footer'
import bookContent from './components/content/article_01-01'
export default {
  name: 'app',
  components: {
    'book-header-nav': bookHeader,
    'book-side-nav': bookSider,
    'book-footer': bookFooter,
    'book-content': bookContent
  }
}
</script>

<style>

  body {
      background-color: #F3F3F3 !important;
  }

  #wrapper {
    width: 100%;
    padding: 0;
    margin: 0;
  }
  .main {
    margin: 90px 20px 70px 230px;
    padding: 25px;
    border: 1px solid #E3E3E3;
    background: #fff;
  }
</style>
