<template>
  <main class="main">
    <div class="main-content container">
      <h1>Content goes here</h1>
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

.main {
  width: 100%;
  background-color: #1c1c1c;

  /* test */
  height: 130px;
}

.main-content {
  display: flex;
  align-items: center;

  /* test */
  height: 130px;
}

h1 {
  color: white;
}
</style>
