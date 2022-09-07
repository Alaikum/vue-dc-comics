<template>
  <div class="social__footer">
    <div class="container">
      <span class="input__footer">Sign-up Now!</span>
      <div class="follow__us">
        <h2>Follow US</h2>
        <img v-for="(el,id) in social" :key="id" :src="el.img" :alt="el.text">
      </div>
    </div>


  </div>

</template>

<script>

export default {
  data() {
    return {
      social: [
        {
          img: require("../assets/footer-facebook.png"),
          text: 'Facebook'
        },
        {
          img: require("../assets/footer-twitter.png"),
          text: 'Twitter'
        },
        {
          img: require("../assets/footer-youtube.png"),
          text: 'Youtube'
        },
        {
          img: require("../assets/footer-periscope.png"),
          text: 'Periscope'
        },
        {
          img: require("../assets/footer-pinterest.png"),
          text: 'Pinterest'
        },
      ]
    }
  }


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../style/variables';

.social__footer {
  background-color: #303030;


  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .input__footer {
      cursor: pointer;
      text-transform: uppercase;
      color: white;
      border: 1px solid $blue-dc ;
      padding: 15px;
    }

    .follow__us {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      height: 110px;

      h2 {
        padding: 10px;
        color: $blue-dc;
        cursor: pointer;
      }

      img {
        cursor: pointer;

      }
    }
  }

}
</style>


