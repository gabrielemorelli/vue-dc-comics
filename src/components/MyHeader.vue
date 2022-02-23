<template>
  <header>
    <div class="testata">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>

      <div v-for="(item, index) in items" :key="index" class="lista">
        {{ item.text }}
      </div>
    </div>

    <div class="jumbotron">
      <img src="../assets/img/jumbotron.jpg" alt="">
    </div>
  </header>
</template>

<script>
export default {
  name: "MyHeader",

  data() {
    return {
      items: [
        {
          link: "#",
          text: "CARACTERS",
        },
        {
          link: "#",
          text: "COMICS",
        },
        {
          link: "#",
          text: "MOVIES",
        },
        {
          link: "#",
          text: "TV",
        },
        {
          link: "#",
          text: "TV",
        },
        {
          link: "#",
          text: "GAMES",
        },

        {
          link: "#",
          text: "COLLECTIBILES",
        },
        {
          link: "#",
          text: "VIDEOS",
        },
        {
          link: "#",
          text: "FANS",
        },
        {
          link: "#",
          text: "SHOP",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.testata {
  margin: 0 auto;
  width: 70%;
  height: 120px;
  display: flex;
}

.logo {
  float: left;
  margin-top: 10px;
}
.lista{
  padding: 10px;
  line-height: 120px;
  font-size: 15px;
 
}

.jumbotron{
width: 100%;
}

.jumbotron img{
  object-position:top;
  object-fit: cover;
  height: 100%;
}

</style>
