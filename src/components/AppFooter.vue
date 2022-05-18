<template>
  <footer class="footer">
    <div class="container">
      <!-- Container col sx -->
      <div class="left-col">
        <!-- DC Comics + Shop -->
        <div class="col">
          <div>
            <h3>DC COMICS</h3>
            <ul>
              <li v-for="(item, index) in dcComicsLinks" :key="index">
                {{ item.text }}
              </li>
            </ul>
            <h3>SHOP</h3>
            <ul>
              <li v-for="(item, index) in shopLinks" :key="index">
                {{ item.text }}
              </li>
            </ul>
          </div>
        </div>

        <!-- DC -->
        <div class="col">
          <h3>DC</h3>
          <ul>
            <li v-for="(item, index) in dcLinks" :key="index">
              {{ item.text }}
            </li>
          </ul>
        </div>

        <!-- Sites -->
        <div class="col">
          <h3>SITES</h3>
          <ul>
            <li v-for="(item, index) in sitesLinks" :key="index">
              {{ item.text }}
            </li>
          </ul>
        </div>
      </div>
      <!-- /Container col sx -->

      <!-- Img logo DC -->
      <div class="logoimg">
        <img src="../assets/img/dc-logo-bg.png" alt="dc-logo-bg" />
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
  data: function () {
    return {
      dcComicsLinks: [
        {
          url: "#",
          text: "Characters",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: false,
        },
        {
          url: "#",
          text: "Movies",
          active: false,
        },
        {
          url: "#",
          text: "Tv",
          active: false,
        },
        {
          url: "#",
          text: "Games",
          active: false,
        },
        {
          url: "#",
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
      ],
      shopLinks: [
        {
          url: "#",
          text: "Shop DC",
          active: false,
        },
        {
          url: "#",
          text: "Shop DC Collectibles",
          active: false,
        },
      ],
      dcLinks: [
        {
          url: "#",
          text: "Terms Of Use",
          active: false,
        },
        {
          url: "#",
          text: "Privacy policy (New)",
          active: false,
        },
        {
          url: "#",
          text: "Ad Choices",
          active: false,
        },
        {
          url: "#",
          text: "Advertising",
          active: false,
        },
        {
          url: "#",
          text: "Jobs",
          active: false,
        },
        {
          url: "#",
          text: "Subscription",
          active: false,
        },
        {
          url: "#",
          text: "Talent Workshops",
          active: false,
        },
        {
          url: "#",
          text: "CPSC Certificates",
          active: false,
        },
        {
          url: "#",
          text: "Ratings",
          active: false,
        },
        {
          url: "#",
          text: "Shop Help",
          active: false,
        },
        {
          url: "#",
          text: "Contact Us",
          active: false,
        },
      ],
      sitesLinks: [
        {
          url: "#",
          text: "DC",
          active: false,
        },
        {
          url: "#",
          text: "Mad Magazines",
          active: false,
        },
        {
          url: "#",
          text: "DC Kids",
          active: false,
        },
        {
          url: "#",
          text: "DC Universe",
          active: false,
        },
        {
          url: "#",
          text: "DC Power Visa",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.footer {
  width: 100%;
  background-image: url(../assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
}

h3 {
  padding: 1rem 0;
  color: white;
}

ul {
  display: flex;
  flex-direction: column;
}

li {
  margin: 0.3rem 0;
  color: rgba($color: #ffffff, $alpha: 0.6);
  font-weight: lighter;
}

.left-col {
  display: flex;
}

.col {
  display: inline-block;
  padding-top: 1.5rem;
  margin-right: 2rem;
}

.container {
  display: flex;
  justify-content: space-between;
  position: relative;
  padding: 1.8rem 0;
}

.logoimg {
  position: absolute;
  right: 0;
  bottom: -5rem;
  overflow: hidden;
  z-index: 0;
}
</style>
