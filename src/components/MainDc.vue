<template>
  <main>
    <div class="container">
      <h2>
        Coming Soon
      </h2>
    </div>
   <BlueShopZone/>
  </main>
</template>

<script>
import BlueShopZone from '../components/BlueShopZone.vue';
export default {
    components: {
      BlueShopZone
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
main {
  background-color: black;
  color: white;
  height:285px;
  font-size: 2rem;

  h2{
      line-height: 130px;
  }
}
</style>
