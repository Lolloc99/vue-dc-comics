<template>
  <main class="footer-bottom">
    <div class="footer-bottom-content container">
      <button>Sign-up Now</button>

      <div class="social-container">
        <h2>FOLLOW US</h2>
        <img src="../assets/img/footer-facebook.png" alt="facebook" />
        <img src="../assets/img/footer-youtube.png" alt="youtube" />
        <img src="../assets/img/footer-twitter.png" alt="twitter" />
        <img src="../assets/img/footer-pinterest.png" alt="pinterest" />
        <img src="../assets/img/footer-periscope.png" alt="periscope" />
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "AppMain",
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.footer-bottom {
  width: 100%;
  background-color: #303030;
  padding: 2.07rem 0;
  position: relative;
  z-index: 1;
}

.footer-bottom-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

button {
  color: white;
  padding: 1rem;
  font-weight: bold;
  font-size: 1rem;
  border: 2px solid #0282f9;
  background-color: #303030;
  text-transform: uppercase;
  cursor: pointer;
}

.social-container {
  display: flex;
  align-items: center;

  h2 {
    color: #0282f9;
    margin-right: 0.5rem;
    font-size: 1.4rem;
  }

  img {
    margin: 0 0.7rem;
  }
}
</style>
