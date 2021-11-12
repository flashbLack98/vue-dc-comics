<template>
  <footer>
    <div class="background_blue">
      <div class="container_item">
        <div v-for="(item, i) in linkBlue" :key="i" class="item">
          <div>
            <img :src="item.img" :alt="item.title" />
          </div>
          <h5>{{ item.title }}</h5>
        </div>
      </div>
    </div>
    <div class="background_superheros">
      <div class="container_linkDClogo">
        <div class="container_link">
          <div class="link_item">
            <h4>DC COMICS</h4>
            <ul>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
            </ul>
            <h4>DC COMICS</h4>
            <ul>
              <li>characters</li>
              <li>characters</li>
            </ul>
          </div>
          <div class="link_item">
            <h4>DC COMICS</h4>
            <ul>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
            </ul>
          </div>
          <div class="link_item">
            <h4>DC COMICS</h4>
            <ul>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
              <li>characters</li>
            </ul>
          </div>
        </div>
        <img src="../assets/dc-logo-bg.png" alt="" />
      </div>
    </div>
    <div class="background_social">
      <div class="social_container">
        <button>SIGN-UP NOW</button>

        <ul>
          <li><h4>FOLLOW US</h4></li>
          <li><img src="../assets/footer-facebook.png" alt="" /></li>
          <li><img src="../assets/footer-twitter.png" alt="" /></li>
          <li><img src="../assets/footer-youtube.png" alt="" /></li>
          <li><img src="../assets/footer-pinterest.png" alt="" /></li>
          <li><img src="../assets/footer-periscope.png" alt="" /></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      linkBlue: [
        {
          img: require("../assets/buy-comics-digital-comics.png"),
          title: "DIGITAL COMICS",
        },
        {
          img: require("../assets/buy-comics-merchandise.png"),
          title: "DC MERCHANDISE",
        },
        {
          img: require("../assets/buy-comics-subscriptions.png"),
          title: "SUBSCRIPTION",
        },
        {
          img: require("../assets/buy-comics-shop-locator.png"),
          title: "COMIC SHOP LOCATOR",
        },
        {
          img: require("../assets/buy-dc-power-visa.svg"),
          title: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.background_blue {
  background-color: #0282f9;
  position: relative;
  z-index: 1;
  .container_item {
    display: flex;
    justify-content: space-around;
    width: 1000px;
    margin: auto;

    .item {
      padding: 50px 0;
      display: flex;
      align-items: center;
      div {
        height: 50px;
        width: 50px;

        img {
          height: 100%;
          width: 100%;
          object-fit: contain;
        }
      }
      h5 {
        color: white;
      }
    }
  }
}

.background_superheros {
  background-image: url("../assets/footer-bg.jpg");
  background-size: cover;

  .container_linkDClogo {
    width: 1000px;
    margin: auto;
    display: flex;
    position: relative;
    .container_link {
      display: flex;
      width: 50%;
      padding-top: 40px;
      flex-wrap: wrap;
      .link_item {
        width: calc(100% / 3);
        h4 {
          margin: 0;
          color: white;
        }

        ul {
          padding: 0;
          list-style: none;
          color: gray;
        }
      }
    }

    img {
      height: 100%;
      position: absolute;
      transform: scale(1.5);
      top: 0;
      right: 0;
    }
  }
}

.background_social {
  background-color: #303030;
  position: relative;
  z-index: 1;
  .social_container {
    width: 1000px;
    margin: auto;
    display: flex;
    align-content: center;
    justify-content: space-between;
    padding: 30px 0;
    .button_box {
      button {
        background-color: black;
      }
    }

    ul {
      list-style: none;
      margin: 0;
      padding: 0;
      li {
        display: inline-block;
        vertical-align: middle;
        padding: 0 10px;
        h4 {
          color: #0282f9;
          margin: 0;
        }
      }
    }
  }
}
</style>