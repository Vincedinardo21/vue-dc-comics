<template>
    <header>
        <!-- <h1>Questo è l'header</h1> -->
        <a href="#">
          <img src="../assets/img/dc-logo.png" alt="dc logo">
        </a>
        <nav>
          <ul>
            <li v-for="(item, i) in navElements" :key="i" :class="item.current ? 'here' : '' ">
              <a href="item.url">{{item.text}}</a>
            </li>
          </ul>
        </nav>
    </header>
</template>

<script>
export default {
  name: 'MyHeader',
  data(){
    return {
      navElements : [
        {
          text : "CHARACTERS",
          url : "#",
          current : false
        },
        {
          text : "COMICS",
          url : "#",
          current : true
        },
        {
          text : "MOVIES",
          url : "#",
          current : false
        },
        {
          text : "TV",
          url : "#",
          current : false
        },
        {
          text : "GAMES",
          url : "#",
          current : false
        },
        {
          text : "COLLECTIBLES",
          url : "#",
          current : false
        },
        {
          text : "VIDEOS",
          url : "#",
          current : false
        },
        {
          text : "FANS",
          url : "#",
          current : false
        },
        {
          text : "NEWS",
          url : "#",
          current : false
        },
        {
          text : "SHOP",
          url : "#",
          current : false
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  width: 70%;
  margin: 0 auto;
  //border: 1px solid black;
  display: flex;
  justify-content: space-between;
  align-items: center;
  
  nav {
    ul {
    list-style-type: none;
    height: 150px;
    

      li {
        display: inline-block;
        padding: 10px;
        
        //border: 1px solid red;
        height: 100%;

          &.here {
            //background-color: aqua;
            border-bottom: 6px solid rgb(2, 130, 249);
          }

            a {
            text-decoration: none;
            color: black;
      
      
              &:hover {
                color: blue;
              }
            }
      }   
    }
  }
  
}
</style>