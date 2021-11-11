<template>
  <div>
    <div class="container_header">
      <img src="../assets/dc-logo.png" alt="logo DC" />
      <ul>
        <li>CHARACTERS</li>
        <li>COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
div {
  .container_header {
    width: 1000px;
    display: flex;
    margin: auto;
    align-items: center;
    justify-content: space-between;
    img {
      padding-bottom: 10px;
    }
    ul {
      list-style: none;
      li {
        display: inline-block;
        font-size: 10px;
        padding: 0 10px;
        font-weight: bold;
      }
    }
  }
}
</style>