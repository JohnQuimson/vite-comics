<script>
export default {
  name: 'Shop',
  data() {
    return {
      shopElements: [
        {
          nome: 'digital comics',
          link: '#',
          foto: '/img/buy-comics-digital-comics.png',
        },
        {
          nome: 'dc merchandise',
          link: '#',
          foto: '/img/buy-comics-merchandise.png',
        },
        {
          nome: 'subscription',
          link: '#',
          foto: '/img/buy-comics-subscriptions.png',
        },
        {
          nome: 'comic shop locator',
          link: '#',
          foto: '/img/buy-comics-shop-locator.png',
        },
        {
          nome: 'dc power visa',
          link: '#',
          foto: '/img/buy-dc-power-visa.svg',
        },
      ],
    };
  },
};
</script>

<template>
  <section class="shop">
    <ul>
      <li v-for="(li, index) in shopElements">
        <div class="cont-shop-icons">
          <img
            :src="`../../public/${li.foto}`"
            :alt="`img-shop-${index + 1}`"
          />
        </div>
        <a :href="li.link">
          <span>{{ li.nome }}</span>
        </a>
      </li>
    </ul>
  </section>
</template>

<style scoped></style>
