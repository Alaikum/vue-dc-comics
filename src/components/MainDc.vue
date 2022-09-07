<template>
  <main>
    <JumboHero />
    <div class="container">
      <button class="button">current series</button>
      <button class="load__button">load more</button>
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
import JumboHero from '../components/JumboHero.vue';


export default {
  components: {
    BlueShopZone,
    HeroCards,
    JumboHero
  },
  data() {
    return {
      cards
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../style/variables';

main {
  background-color: #1C1C1C;
  color: white;
  // height:285px;
  font-size: 13px;
  text-transform: uppercase;


  .container {
    padding-top: 50px;
    position: relative;
    height: 670px;

    .button {
      position: absolute;
      top: 0;
      transform: translateY(-50%);
      font-size: 25px;
      font-weight: bold;
      text-transform: uppercase;
      padding: 10px;
      color: white;
      background-color: $blue-dc;
      cursor: pointer;
    }

    .load__button {
      position: absolute;
      color: white;
      background-color: $blue-dc;
      font-size: 16px;
      font-weight: bold;
      text-transform: uppercase;
      padding: 10px 40px;
      cursor: pointer;
      bottom: 20px;
      left: 50%;
      transform: translateX(-50%);

    }

    .cards {
      display: grid;
      grid-template-columns: repeat(6, 1fr);
      gap: 30px;
      padding: 0 20px;


    }
  }
}
</style>
