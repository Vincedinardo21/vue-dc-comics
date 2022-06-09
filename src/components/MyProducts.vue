<template>
    <section>
        <div class="card">
            <img src="../assets/img/buy-comics-merchandise.png" alt="nome">
            <div>Name</div>
        </div>
    </section>   
</template>

<script>
export default {
  name: 'MyProducts',
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
    section {
        background-color: violet;
    }
</style>