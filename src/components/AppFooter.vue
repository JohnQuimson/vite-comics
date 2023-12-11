<script>
import FooterTop from './FooterTop.vue';

export default {
  name: 'Footer',
  data() {
    return {
      socialIcons: [
        {
          foto: 'img/footer-facebook.png',
          link: '#',
        },
        {
          foto: 'img/footer-twitter.png',
          link: '#',
        },
        {
          foto: 'img/footer-youtube.png',
          link: '#',
        },
        {
          foto: 'img/footer-pinterest.png',
          link: '#',
        },
        {
          foto: 'img/footer-periscope.png',
          link: '#',
        },
      ],
    };
  },
  components: {
    FooterTop,
  },
};
</script>

<template>
  <FooterTop />
  <footer>
    <div class="footer-sx">
      <button>sign-up now!</button>
    </div>
    <div class="footer-dx">
      <ul>
        <li>
          <a href="#">
            <span>Follow us</span>
          </a>
        </li>
        <li v-for="li in socialIcons">
          <a :href="li.link">
            <img :src="`../../public/${li.foto}`" alt="" />
          </a>
        </li>
      </ul>
    </div>
  </footer>
</template>

<style lang="scss">
footer {
  height: 12vh;
  background-color: #303030;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 200px;

  .footer-sx {
    button {
      background-color: #303030;
      border: 2px solid #0282f9;
      color: white;
      padding: 10px;
      text-transform: uppercase;
      font-size: 12px;
    }
  }

  .footer-dx {
    ul {
      display: flex;
      list-style-type: none;
      align-items: center;
      gap: 20px;

      a {
        text-decoration: none;
      }

      span {
        text-transform: uppercase;
        color: #0282f9;
        font-weight: 600;
      }

      img {
        height: 30px;
      }
    }
  }
}
</style>
