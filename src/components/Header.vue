<template>
  <header>
    <div class="container_header">
      <img src="../assets/dc-logo.png" alt="logo DC" />
      <ul>
        <li v-for="(item, i) in navbarItems" :key="i">{{ item.title }}</li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      navbarItems: [
        {
          title: "CHARCTERS",
          href: "#",
        },
        {
          title: "COMICS",
          href: "#",
        },
        {
          title: "MOVIES",
          href: "#",
        },
        {
          title: "TV",
          href: "#",
        },
        {
          title: "GAMES",
          href: "#",
        },
        {
          title: "COLLECTIBLES",
          href: "#",
        },
        {
          title: "VIDEO",
          href: "#",
        },
        {
          title: "FANS",
          href: "#",
        },
        {
          title: "NEWS",
          href: "#",
        },
        {
          title: "SHOP",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
div {
  .container_header {
    width: 1000px;
    display: flex;
    margin: auto;
    align-items: center;
    justify-content: space-between;
    padding-top: 10px;
    img {
      padding-bottom: 10px;
    }
    ul {
      list-style: none;
      margin: 0;
      padding: 0;
      li {
        display: inline-block;
        font-size: 10px;
        padding: 0 5px;
        font-weight: bold;
      }
    }
  }
}
</style>