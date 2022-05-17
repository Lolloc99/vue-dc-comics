<template>
  <div class="bonus">
    <div class="bonus-content container">
      <ul>
        <li v-for="(item, index) in bonusLinks" :key="index">
          <img :src="require(`../assets/img/${item.image}`)" :alt="item.text" />
          <h3>{{ item.text }}</h3>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppBonus",
  data: function () {
    return {
      bonusLinks: [
        {
          image: "buy-comics-digital-comics.png",
          text: "Digital Comics",
        },
        {
          image: "buy-comics-merchandise.png",
          text: "DC Merchandise",
        },
        {
          image: "buy-comics-subscriptions.png",
          text: "Subscription",
        },
        {
          image: "buy-comics-shop-locator.png",
          text: "Comic Shop Locator",
        },
        {
          image: "buy-dc-power-visa.svg",
          text: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.bonus {
  width: 100%;
  background-color: #0282f9;

  /* test */
  height: 150px;
}

.bonus-content {
  display: flex;
  align-items: center;

  /* test */
  height: 150px;
}

.container {
  width: 65%;
}

ul {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

li {
  display: flex;
  align-items: center;

  img {
    display: inline-block;
    width: 50px;
    margin-right: 1rem;
  }

  h3 {
    display: inline-block;
    color: white;
    text-transform: uppercase;
    font-weight: lighter;
  }
}
</style>
