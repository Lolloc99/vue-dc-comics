<template>
  <header class="header">
    <div class="header-content container">
      <div class="header-img">
        <img src="../assets/img/dc-logo.png" alt="dc-logo." />
      </div>
      <div>
        <ul>
          <li v-for="(item, index) in HeaderLinks" :key="index">
            {{ item.text }}
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      HeaderLinks: [
        {
          url: "#",
          text: "Characters",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: true,
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
          text: "Collectibles",
          active: false,
        },
        {
          url: "#",
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "Fans",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
        {
          url: "#",
          text: "Shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.header {
  width: 100%;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;

  .header-img img {
    display: inline-block;
    width: 80%;
  }
}

li {
  font-weight: bold;
  line-height: 100px;
  margin: 0.7rem;
  border-bottom: 5px solid transparent;
  text-transform: uppercase;
}
</style>
