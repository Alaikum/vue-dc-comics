<template>
  <nav>
    <div class="container">
      <figure>
        <img src="../assets/dc-logo.png" alt="Logo">
      </figure>

      <ul>
        <li>
          <a href="">
            characters
          </a>
        </li>
        <li class="active">
          <a href="">
            comics
          </a>
        </li>
        <li>
          <a href="">
            movies
          </a>
        </li>
        <li>
          <a href="">
            tv
          </a>
        </li>
        <li>
          <a href="">
            games
          </a>
        </li>
        <li>
          <a href="">
            collectibles
          </a>
        </li>
        <li>
          <a href="">
            videos
          </a>
        </li>
        <li>
          <a href="">
            fans
          </a>
        </li>
        <li>
          <a href="">
            news
          </a>
        </li>
        <li>
          <a href="">
            shop
          </a>
        </li>
      </ul>

    </div>
  </nav>
</template>

<script>
export default {

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
  padding-bottom: 1.25rem;

  figure{
    max-width: 82px;
  }
  ul {
    display: flex;
    justify-content: space-between;
    gap: 30px;
    text-transform: uppercase;
    font-size: 12px;
    font-weight: bold;

    li {
      padding: 1rem 0;

      &.active, &:hover {
        color: $blue-dc;
        border-bottom: 3px solid $blue-dc;

      }
    }

  }
}
</style>
