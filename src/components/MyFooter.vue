<template>
    <footer>
        <!-- Footer Up -->
        <section class="footer-up">
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

        <!-- Footer Middle -->
        <section class="footer-middle">
          <div class="list-container">
            <!-- Left List -->
            <ul>
              <li><h2>DC COMICS</h2></li>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>

              <li><h2>SHOP</h2></li>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>

            <!-- Center List -->
            <ul>
              <li><h2>DC</h2></li>
              <li>Terms Of Us</li>
              <li>Privacy policy (New)</li>
              <li>Add Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>

            <!-- Right List -->
            <ul>
              <li><h2>SITES</h2></li>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
          
        </section>

        <!-- Footer Bottom -->
        <section class="footer-bottom">
          <div class="bottom-container">
            <div class="sign-up">
              <a href="#">SIGN UP NOW!</a>            
            </div>
            <ul>
              <li><h2 class="follow">FOLLOW US</h2></li>
              <li><img src="../assets/img/footer-facebook.png" alt="facebook icon"></li>
              <li><img src="../assets/img/footer-twitter.png" alt="twitter icon"></li>
              <li><img src="../assets/img/footer-youtube.png" alt="youtube icon"></li>
              <li><img src="../assets/img/footer-pinterest.png" alt="pinterest icon"></li>
              <li><img src="../assets/img/footer-periscope.png" alt="periscope icon"></li>
            </ul>
          </div>        
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
  //background-color: aqua;
  a {
    color: white;
    text-decoration: none;
  }

  ul{
    margin-right: 40px;
    &.product{
      display: flex;
      justify-content: space-around;
      align-items:center;

      div {
        display: flex;
        align-items: center;
      }
    }
    
  }
  
  .product, .list-container, .bottom-container{
    width: 70%;
    margin: 0 auto;
    padding: 30px 0;
  }

 

  .footer-up {
    background-color: rgb(2, 130, 249);
  }

  section{
    &.footer-middle {
      h2 {
        color: white;
      }
      background-image: url("../assets/img/footer-bg.jpg");
      background-repeat: no-repeat;
      background-size: cover;
      //border: 1px solid black;
      min-height: 100px;

       .list-container{
         display: flex;
         
         li {
           color: gray;
         }
       }
    }
  }

  section{
    &.footer-bottom {
      
      background-color: rgb(48, 48, 48);
      min-height: 100px;

      .bottom-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
      }

      .sign-up {
        padding: 20px;
        border: 1px solid rgb(2, 130, 249);
      }

      ul{
        display: flex;
        justify-content: space-around;
        align-items: center;

        li{
          margin-right: 10px;

          .follow{
            color: rgb(2, 130, 249);
          }
        }
      }
    }
  }
}
</style>