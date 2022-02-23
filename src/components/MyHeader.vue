<template>
  <header>
    <div class="testata">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <div class="menu-list">
        <div v-for="(item, index) in items" :key="index" class="lista">
          {{ item.text }}
        </div>
      </div>
    </div>

    <div class="jumbotron">
      
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
 
}

.logo {
  float: left;
  margin-top: 10px;
  width: 20%;
}

.menu-list {
  display: flex;
  justify-content: flex-end;
  width: 80%;
}
.lista {
  padding: 10px;
  line-height: 120px;
  font-size: 15px;
}

.jumbotron {
 height: 350px;
  background-image: url('../assets/img/jumbotron.jpg');
  background-position: top;
background-size: cover;
}


</style>
