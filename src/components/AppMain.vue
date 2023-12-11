<script>
import Jumbotron from './Jumbotron.vue';
import Films from './Films.vue';

export default {
  name: 'Main',
  components: {
    Jumbotron,
    Films,
  },
};
</script>

<template>
  <main>
    <Jumbotron />
    <Films />
  </main>
</template>

<style lang="scss" scoped>
main {
  background-color: #1c1c1c;
  color: white;
  display: flex;
  flex-direction: column;
}
</style>
