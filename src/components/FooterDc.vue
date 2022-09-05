<template>
  <footer>
    <div class="container">
      <div class="main__footer">
        <div class="ul__footer">
          <ul>
            <h2>Dc comics</h2>
            <li v-for="el in dcComics" :key="el.id">
              <a href="">
                {{ el }}
              </a>
            </li>
          </ul>
          <ul>
            <h2>Shop</h2>
            <li v-for="el in shop" :key="el.id">
              <a href="">
                {{ el }}
              </a>
            </li>
          </ul>
          <ul>
            <h2>Dc</h2>
            <li v-for="el in dc" :key="el.id">
              <a href="">
                {{ el }}
              </a>
            </li>
          </ul>
          <ul>
            <h2>Sites</h2>
            <li v-for="el in sites" :key="el.id">
              <a href="">
                {{ el }}
              </a>
            </li>
          </ul>
        </div>
        <figure>
          <img src="../assets/dc-logo-bg.png" alt="">
        </figure>
      </div>
    </div>
    <SocialDc />
  </footer>
</template>

<script>
import SocialDc from './SocialDc.vue';
export default {
  components: { SocialDc },
  data() {
    return {
      dcComics: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'],
      shop: ['Shop DC', 'Shop DC Collectibles'],
      dc: ['Terms Of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us'],
      sites: ['Dc', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa'],
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
footer {
  background-image: url(../assets/footer-bg.jpg);
  background-size: cover;
  background-position: center;

  .main__footer {
    display: flex;
    justify-content: space-between;


    .ul__footer {
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;
      max-height: 370px;
      gap: 30px;
      padding-top: 30px;

      ul {
        color: white;

        h2 {
          font-size: 18px;
          text-transform: uppercase;
          padding-bottom: 10px;
        }

        li {
          color: grey;
          padding-bottom: 10px;
          font-size: 12px;

          &:hover {
            color: white;
            cursor: pointer;
          }
        }
      }
    }

    figure {
      max-height: 370px;
      overflow: hidden;

      img {
        transform: translateY(-20%);
      }
    }
  }
}
</style>
