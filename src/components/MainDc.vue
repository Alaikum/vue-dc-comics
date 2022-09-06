<template>
  <main>
    <div class="container">
      <div class="cards">

        <HeroCards v-for="(slide, i) in cards" :key="i" :thumb="slide.thumb" :series="slide.series" />

      </div>
    </div>
    <BlueShopZone />
  </main>
</template>

<script>
import BlueShopZone from '../components/BlueShopZone.vue';
import HeroCards from '../components/HeroCards.vue';
import cards from '../myscript';
export default {
  components: {
    BlueShopZone,
    HeroCards
  },
  data() {
    return {
      cards
    }
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
main {
  background-color: black;
  color: white;
  // height:285px;
  font-size: 2rem;

  .cards {
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    gap: 10px;
    
  }
}
</style>
