<script>
export default {
  name: 'FooterTop',
  data() {
    return {
      list1: [
        {
          title: 'dc comics',
        },
        {
          title: 'Characters',
          link: '#',
        },
        {
          title: 'Comics',
          link: '#',
        },
        {
          title: 'Movies',
          link: '#',
        },
        {
          title: 'TV',
          link: '#',
        },
        {
          title: 'Games',
          link: '#',
        },
        {
          title: 'Videos',
          link: '#',
        },
        {
          title: 'News',
          link: '#',
        },
      ],
      list2: [
        {
          title: 'shop ',
        },
        {
          title: 'Shop DC',
          link: '#',
        },
        {
          title: 'Shop DC Collectibles',
          link: '#',
        },
      ],
      list3: [
        {
          title: 'dc',
        },
        {
          title: 'Term of Use',
          link: '#',
        },
        {
          title: 'Privacy policy (New)',
          link: '#',
        },
        {
          title: 'Ad Choices',
          link: '#',
        },
        {
          title: 'Advertising',
          link: '#',
        },
        {
          title: 'Jobs',
          link: '#',
        },
        {
          title: 'Subscriptions',
          link: '#',
        },
        {
          title: 'Talent Workshops',
          link: '#',
        },
        {
          title: 'CPSC Certificates',
          link: '#',
        },
        {
          title: 'Ratings',
          link: '#',
        },
        {
          title: 'Shop Help',
          link: '#',
        },
        {
          title: 'Contact Us',
          link: '#',
        },
      ],
      list4: [
        {
          title: 'sites',
        },
        {
          title: 'DC',
          link: '#',
        },
        {
          title: 'MAD Magazine',
          link: '#',
        },
        {
          title: 'DC Kids',
          link: '#',
        },
        {
          title: 'DC Universe',
          link: '#',
        },
        {
          title: 'DC Power Visa',
          link: '#',
        },
      ],
    };
  },
};
</script>

<template>
  <section class="footer-top">
    <div class="cont-list">
      <div class="col1">
        <ul>
          <li v-for="li in list1">
            <a :href="li.link">
              <span>{{ li.title }}</span>
            </a>
          </li>
        </ul>
        <ul>
          <li v-for="li in list2">
            <a :href="li.link">
              <span>{{ li.title }}</span>
            </a>
          </li>
        </ul>
      </div>
      <div class="col2">
        <ul>
          <li v-for="li in list3">
            <a :href="li.link">
              <span>{{ li.title }}</span>
            </a>
          </li>
        </ul>
      </div>
      <div class="col3">
        <ul>
          <li v-for="li in list4">
            <a :href="li.link">
              <span>{{ li.title }}</span>
            </a>
          </li>
        </ul>
      </div>
    </div>
    <div class="cont-img">
      <img src="../../public/img/dc-logo-bg.png" alt="" />
    </div>
  </section>
</template>

<style lang="scss">
.footer-top {
  background-image: url(../../public/img/footer-bg.jpg);
  height: 42vh;
  color: #fffdfe;
  overflow: hidden;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 200px;

  .cont-list {
    display: flex;
    gap: 30px;

    ul {
      list-style-type: none;
      letter-spacing: 0.5px;
      margin-bottom: 20px;

      li {
        &:first-child {
          margin-bottom: 12px;
        }

        &:first-child a {
          color: #fffdfe;
          text-transform: uppercase;
          font-size: 18px;
        }

        a {
          color: #959595;
          text-decoration: none;
          font-size: 12px;
        }
      }
    }
  }
}
</style>
