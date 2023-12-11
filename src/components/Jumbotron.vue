<script>
export default {
  name: 'Jumbotron',
};
</script>

<template>
  <section>
    <div class="cont-jumbo">
      <img src="../../public/img/jumbotron.jpg" alt="" />
    </div>
  </section>
</template>

<style lang="scss" scoped>
.cont-jumbo {
  height: 400px;
  width: 100%;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top;
  }
}
</style>
