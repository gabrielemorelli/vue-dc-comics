<template>
  <footer>
    <!--footer top-->
    <div class="footer-top">
      <div class="row">
        <div v-for="(item, index) in items" :key="index" class="box">
          <a href="#"><img :src="item.img" alt="#"></a>
          {{ item.text }}
        </div>

        <!--
        <div class="comics">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
          <div class="text">
        Digital Comics
          </div>
        
        </div>

 
        <div class="merchandise">
          <img src="../assets/img/buy-comics-merchandise.png" alt="" />
          <span>DC Merchandise</span>
        </div>

        <div class="substription">
          <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
          <span>subscriptions</span>
        </div>

        <div class="Comic-Shop-Locator">
          <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
          <span>Comic shop locator</span>
        </div>

        <div class="dc-power-usa">
          <img src="../assets/img/buy-dc-power-visa.svg" alt="" />
          <span>DC power visa</span>
        </div>
       -->

      </div>
    </div>

    <!--/footer top-->

    <!--inizio footer-center-->
    <div class="footer-center">
      <div class="row-2">
        <div class="footer-list">
        
          <div class="lista">
            <h3>Dc comics</h3>
            <ul>
              <li><a href="#">characters</a></li>
              <li><a href="#">comics</a></li>
              <li><a href="#">moies</a></li>
              <li><a href="#">tv</a></li>
              <li><a href="#">games</a></li>
              <li><a href="#">videos</a></li>
              <li><a href="#">news</a></li>
            </ul>
            <h3>shop</h3>
            <ul>
              <li><a href="#">shop dc</a></li>
              <li><a href="#">shop dc collections</a></li>
            </ul>
          </div>

          <div class="lista">
            <h3>Dc comics</h3>
            <ul>
              <li><a href="#">characters</a></li>
              <li><a href="#">comics</a></li>
              <li><a href="#">moies</a></li>
              <li><a href="#">tv</a></li>
              <li><a href="#">games</a></li>
              <li><a href="#">videos</a></li>
              <li><a href="#">news</a></li>
            </ul>
          </div>

          <div class="lista">
            <h3>Dc comics</h3>
            <ul>
              <li><a href="#">characters</a></li>
              <li><a href="#">comics</a></li>
              <li><a href="#">moies</a></li>
              <li><a href="#">tv</a></li>
              <li><a href="#">games</a></li>
              <li><a href="#">videos</a></li>
              <li><a href="#">news</a></li>
            </ul>
          </div>
        </div>
  
        <div class="footer-img">
          <img src="../assets/img/dc-logo-bg.png" />
        </div>
      </div>
    </div>
    <!--fine  footer-center-->

    <!--inizio footer-bottom-->
    <div class="footer-bottom">
      <div class="footer-menu">
        <div class="menu-social">
          <span>Follow us</span>
          <a href="#"> <img src="../assets/img/footer-facebook.png" /></a>
          <a href="#"> <img src="../assets/img/footer-periscope.png" /></a>
          <a href="#"> <img src="../assets/img/footer-pinterest.png" /></a>
          <a href="#"><img src="../assets/img/footer-twitter.png" /></a>
          <a href="#"><img src="../assets/img/footer-youtube.png" /></a>
        </div>
        <div class="bottone">
          <a href="#" class="btn"> SIGN-UP NOW </a>
        </div>
      </div>
    </div>
    <!--fine  footer-bottom-->
  </footer>
</template>

<script>
export default {
  name: "MyFooter",

  data() {
    return {
      items: [
        {
          img: require("../assets/img/buy-comics-digital-comics.png"),
          text: "Digital Comics",
        },
        {
          img: require("../assets/img/buy-comics-merchandise.png"),
          text: "DC Merchandise",
        },
        {
          img: require("../assets/img/buy-comics-subscriptions.png"),
          text: "subscriptions",
        },
        {
          img: require("../assets/img/buy-comics-shop-locator.png"),
          text: "Comic shop locator",
        },
        {
          img: require("../assets/img/buy-dc-power-visa.svg"),
          text: "DC power visa",
        },
      ],



      
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/variables.scss";

footer {
  background-color: $primarycolor;
}
/*footer-top*/

.footer-top {
  margin: 0 auto;
  width: 70%;
}

.row {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 200px;
}

.footer-top img {
  width: 50px;
  vertical-align: middle;
}


/*footer-top*/

/*footer-center*/
.footer-center {
  background-image: url("../assets/img/footer-bg.jpg");
}

.row-2 {
  width: 70%;
  margin: 0 auto;
  display: flex;
  height: 400px;
}

.lista h3 {
  color: white;
  padding: 15px 0px;
  text-transform: uppercase;
}

.lista {
  float: left;
  width: 150px;
  margin-top: 50px;
}

.lista li {
  list-style-type: none;
}

.lista li a {
  list-style-type: none;
  text-decoration: none;
  color: lightgray;
  line-height: 20px;
}

.footer-img {
  position: relative;
  left: 300px;
  width: 500px;
  overflow: hidden;
}

.footer-center img {
  position: absolute;
  top: -50px;
  width: 100%;
}
/*.footer-center*/

/*footer-bottom*/
.footer-bottom {
  width: 100%;
  background-color: #303030;
}

.btn {
  padding: 16px 32px;
  border: 2px solid $primarycolor;
  color: white;
  text-decoration: none;
}

.footer-menu {
  width: 70%;
  margin: 0 auto;
  height: 150px;
  line-height: 150px;
}

.menu-social a {
  padding: 10px;
}

.menu-social span {
  color: $primarycolor;
  text-transform: uppercase;
 
}

.menu-social {
  float: right;
}

.bottone {
  float: left;
}

/*.footer-bottom*/
</style>
