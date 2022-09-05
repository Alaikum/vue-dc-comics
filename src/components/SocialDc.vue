<template>
  <div class="social__footer">
    <div class="container">
      <span class="input__footer">Sign-up Now!</span>
      <div class="follow__us">
        <h2>Follow US</h2>
        <!-- <img :src="`../assets/${facebook}`" alt="MMMMs"> -->
        <img src="../assets/footer-facebook.png" alt="Facebook" >
        <img src="../assets/footer-twitter.png" alt="Twitter" >
        <img src="../assets/footer-youtube.png" alt="YouTube" >
        <img src="../assets/footer-periscope.png" alt="Periscope" >
        <img src="../assets/footer-pinterest.png" alt="Pinterest" >
      </div>
    </div>


  </div>

</template>

<script>

export default {
  data(){
    return{
      facebook:'footer-facebook.png'
    }
  }


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import '../style/variables';
.social__footer {
  background-color: #303030;
  

  .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    .input__footer{
      cursor: pointer;
      text-transform: uppercase;
      color: white;
      border: 1px solid $blue-dc ;
      padding: 15px;
    }

    .follow__us{
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      height: 110px;

      h2{
        padding: 10px;
        color: $blue-dc
      }
    }
  }

}
</style>


