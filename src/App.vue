<template>
  <div id="app">   
    <MyHeader/>

    <main>
      <!-- <h2>Contenuto Main</h2> -->
      <div class="jumbotron">

      </div>
      <MyProducts/>
    </main>

    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyFooter from './components/MyFooter.vue'
import MyProducts from './components/MyProducts.vue'


export default {
  name: 'App',
  components: {
    MyHeader,
    MyFooter,
    MyProducts
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  //margin-top: 60px;
  // width: 80%;
  // margin: 0 auto;
  ul {
    list-style-type: none;
  }

  // a {
  //   color: white;
  //   text-decoration: none;
  // }

  h2 {
    margin: 20px 0;
  }

  .jumbotron {
    height: 450px;
    background-image: url("assets/img/jumbotron.jpg");
    //background-position: center;
  }
}
</style>
