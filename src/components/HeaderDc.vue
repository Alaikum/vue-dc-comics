<template>
  <nav>
    <div class="container">
      <figure>
        <img src="../assets/dc-logo.png" alt="Logo">
      </figure>

      <ul>
        <li v-for="(link,id) in links" :key="id" :class="id===puntatore ? 'active': ''" @click="puntatore=id">
          <a href="#">
            {{link}}
          </a>
        </li>
       
      </ul>

    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      links: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Collectibles', 'Videos', 'Fans', 'Shop', 'News'],
      puntatore: 1

    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../style/variables';

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 1.25rem;



  figure {
    max-width: 82px;
    padding-bottom: 5px;
  }

  ul {
    display: flex;
    justify-content: space-between;
    gap: 30px;
    text-transform: uppercase;
    font-size: 12px;
    font-weight: bold;
    flex-wrap: wrap;

    li {
      padding: 35px 0;

      &.active,
      &:hover {
        color: $blue-dc;
        border-bottom: 5px solid $blue-dc;
        cursor: pointer;

      }
    }

  }
}
</style>
