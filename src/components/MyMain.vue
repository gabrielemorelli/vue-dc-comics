<template>
  <main>

    <div class="container">
      <div class="title">
        <h2>-->Content goes here--></h2>
      </div>
    </div>

  </main>
</template>

<script>
export default {
  name: "MyMain",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
main {
  background-color: black;
  height: 150px;
}
.container{
  margin: 0 auto;
  width: 70%;
  line-height: 150px;
}

.title h2 {
  color: white;
}
</style>
