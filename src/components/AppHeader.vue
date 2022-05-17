<template>
  <header class="header container">
    <div>
      <img src="../assets/img/dc-logo.png" alt="dc-logo." />
    </div>
    <div>
      <ul>
        <li>prova</li>
        <li>prova</li>
        <li>prova</li>
      </ul>
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
  methods: function () {
      return
  }
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.header {
  display: flex;
  justify-content: space-between;
  background-color: white;
}
</style>
