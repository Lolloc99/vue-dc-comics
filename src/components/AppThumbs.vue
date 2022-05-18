<template>
  <div class="comic-card">
    <div class="card-img">
      <img :src="ComicsObj.thumb" :alt="ComicsObj.series" />
    </div>
    <p>{{ ComicsObj.series }}</p>
  </div>
</template>

<script>
export default {
  name: "ComicsList",
  props: ["ComicsObj"],
};
</script>

<style lang="scss" scoped>
.comic-card {
  display: flex;
  flex-wrap: wrap;
  width: calc(100% / 6);
  margin-bottom: 3rem;
  color: white;

  p {
    max-width: 200px;
  }
}

.card-img {
  width: 100%;
  height: 200px;
  overflow: hidden;
  margin-bottom: 1rem;
}
</style>
