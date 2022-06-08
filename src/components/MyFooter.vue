<template>
    <footer>
        <!-- Footer Up -->
        <section>
          <ul class="product">
            <li v-for="(item, i) in footerElements" :key="i">
              <a href="item.url">
                <!-- immagine e testo -->
                <div>
                  <img :src="item.image" :alt="item.text">
                  <h4>{{item.text}}</h4>
                </div>
              </a>
            </li>
          </ul>
        </section>
    </footer>
</template>

<script>
export default {
  name: 'MyFooter',
  data(){
    return {
      footerElements : [
        {
          text : "DIGITAL COMICS",
          image : require("../assets/img/buy-comics-digital-comics.png"),
          url : "#"
        },
        {
          text : "DC MERCHANDISE",
          image : require("../assets/img/buy-comics-merchandise.png"),
          url : "#"
        },
        {
          text : "SUBSCRIPTION",
          image : require("../assets/img/buy-comics-shop-locator.png"),
          url : "#"
        },
        {
          text : "COMIC SHOP LOCATOR",
          image : require("../assets/img/buy-comics-subscriptions.png"),
          url : "#"
        },
        {
          text : "DC POWER VISA",
          image : require("../assets/img/buy-dc-power-visa.svg"),
          url : "#"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
footer {
  background-color: aqua;

  ul{
    display: flex;
    justify-content: space-around;
    align-items:center;

    div {
      display: flex;
    }
  }
}
</style>