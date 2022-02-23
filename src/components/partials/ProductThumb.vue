<template>
  <div class="product">
      <img :src="product.thumb" :alt="product.series">
       
      <h4>{{product.series}}</h4>

      
  </div>
</template>

<script>
export default {
    name: "ProductThumb",
    props:["product"],

}
</script>

<style scoped lang="scss">

.product{
  width: 15%;
  min-height: 250px;
 padding: 10px;


    h4{
        text-align: center;
        color: white;
    }

    img{
        width: 100%;
    }
}

</style>