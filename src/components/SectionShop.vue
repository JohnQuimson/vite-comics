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

<style lang="scss">
.shop {
  height: 17vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  background-color: #0282f9;
  padding: 0 200px;

  ul {
    display: flex;
    justify-content: space-between;
    list-style-type: none;

    li {
      display: flex;
      align-items: center;
      gap: 20px;

      .cont-shop-icons {
        height: 60px;

        img {
          height: 100%;
          object-fit: contain;
          aspect-ratio: 1;
        }
      }

      a {
        color: #fffdfe;
        text-decoration: none;
        text-transform: uppercase;
        letter-spacing: 0.5px;
      }
    }
  }
}
</style>
