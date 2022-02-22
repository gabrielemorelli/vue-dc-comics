<template>
  <header>
    <div class="testata">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>

      <nav>
        <ul>
          <li>
            <a href="#">CHARACTERS</a>
          </li>
          <li>
            <a href="#">COMICS</a>
          </li>
          <li>
            <a href="#">MOVIES</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">GAMES</a>
          </li>

          <li>
            <a href="#">COLLECTIBILES</a>
          </li>
          <li>
            <a href="#">VIDEOS</a>
          </li>
          <li>
            <a href="#">FANS</a>
          </li>
          <li>
            <a href="#">SHOP</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "MyHeader",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.testata {
  margin: 0 auto;
  width: 70%;
  height: 120px;
}
.logo {
  float: left;
  margin-top: 10px;
}

nav {
  float: right;
  line-height: 120px;
}

li {
  display: inline-block;
  a {
    text-decoration: none;
    color: black;
    padding: 10px;
    font-size: 15px;
  }
}
</style>
