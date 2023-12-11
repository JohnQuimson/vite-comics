<script>
export default {
  name: 'Header',
  data() {
    return {
      navbarElements: [
        {
          nome: 'characters',
          link: '#',
        },
        {
          nome: 'comics',
          link: '#',
        },
        {
          nome: 'movies',
          link: '#',
        },
        {
          nome: 'tv',
          link: '#',
        },
        {
          nome: 'games',
          link: '#',
        },
        {
          nome: 'collectibles',
          link: '#',
        },
        {
          nome: 'videos',
          link: '#',
        },
        {
          nome: 'fans',
          link: '#',
        },
        {
          nome: 'news',
          link: '#',
        },
        {
          nome: 'shop',
          link: '#',
        },
      ],
    };
  },
};
</script>

<template>
  <header>
    <div class="logo">
      <div class="cont-logo">
        <img src="../../public/img/dc-logo.png" alt="" />
      </div>
    </div>
    <ul class="navbar">
      <li v-for="li in navbarElements">
        <span>{{ li.nome }}</span>
      </li>
    </ul>
  </header>
</template>

<style scoped lang="scss">
@use '../assets/scss/main.scss' as *;

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 13vh;
  padding: 0 200px;

  .cont-logo {
    height: 80px;
    width: 80px;

    img {
      width: 100%;
      object-fit: contain;
    }
  }

  .navbar {
    display: flex;
    gap: 20px;
    list-style-type: none;
    letter-spacing: 0.3px;

    span {
      text-transform: uppercase;

      &:hover {
        color: #0282f9;
        cursor: pointer;
      }
    }
  }
}
</style>
