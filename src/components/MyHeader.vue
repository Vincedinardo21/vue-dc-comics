<template>
    <header>
        <!-- <h1>Questo è l'header</h1> -->
        <a href="#">
          <img src="../assets/img/dc-logo.png" alt="dc logo">
        </a>
        <nav>
          <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Home</a></li>
            <li><a href="#">Home</a></li>
          </ul>
        </nav>
    </header>
</template>

<script>
export default {
  name: 'MyHeader',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  border: 1px solid black;

  ul {
    list-style-type: none;

    li {
      display: inline-block;

      a {
      text-decoration: none;
      color: black;
      padding: 10px;
      border: 1px solid red;
      
        &:hover {
          color: blue;
        }
      }
    }   
  }
}
</style>