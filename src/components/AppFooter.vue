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

<style scoped></style>
