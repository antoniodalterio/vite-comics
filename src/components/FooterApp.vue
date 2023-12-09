<script>
import FooterBot from './FooterBot.vue';
export default {
  name: 'topFooter',
  data() {
    return {
      linkFooter1: [
        {
          title: 'DC Comics',
          name: 'Characters',
          link: '#',
          target: '_self',
        },
        {
          name: 'Comics',
          link: '#',
          target: '_self',
        },
        {
          name: 'Movies',
          link: '#',
          target: '_self',
        },
        {
          name: 'Tv',
          link: '#',
          target: '_self',
        },
        {
          name: 'Games',
          link: '#',
          target: '_self',
        },
        {
          name: 'Collectibles',
          link: '#',
          target: '_self',
        },
        {
          name: 'Videos',
          link: '#',
          target: '_self',
        },
        {
          name: 'Fans',
          link: '#',
          target: '_self',
        },
        {
          name: 'News',
          link: '#',
          target: '_self',
        },
        {
          name: 'Shop',
          link: '#',
          target: '_self',
        },
      ],

      linkFooter2: [
        {
          title: 'DC',
          name: 'Terms Of Use',
          link: '#',
          target: '_self',
        },
        {
          name: 'Priacy policy (New)',
          link: '#',
          target: '_self',
        },
        {
          name: 'Ad Choices',
          link: '#',
          target: '_self',
        },
        {
          name: 'Advertising',
          link: '#',
          target: '_self',
        },
        {
          name: 'Jobs',
          link: '#',
          target: '_self',
        },
        {
          name: 'Sunscriptions',
          link: '#',
          target: '_self',
        },
        {
          name: 'Talent Workshops',
          link: '#',
          target: '_self',
        },
        {
          name: 'CPSC Certificates',
          link: '#',
          target: '_self',
        },
        {
          name: 'Rating',
          link: '#',
          target: '_self',
        },
        {
          name: 'Shop Help',
          link: '#',
          target: '_self',
        },
        {
          name: 'Contact us',
          link: '#',
          target: '_self',
        },
      ],

      linkFooter3: [
        {
          title: 'sites',
          name: 'DC',
          link: '#',
          target: '_self',
        },
        {
          name: 'MAD Magazine',
          link: '#',
          target: '_self',
        },
        {
          name: 'DC Kids',
          link: '#',
          target: '_self',
        },
        {
          name: 'DC Universe',
          link: '#',
          target: '_self',
        },
        {
          name: 'DC Power Visa',
          link: '#',
          target: '_self',
        },
      ],

      linkFooter4: [
        {
          title: 'shop',
          name: ' Shop DC',
          link: '#',
          target: '_self',
        },
        {
          name: 'Shop DC Collectibles',
          link: '#',
          target: '_self',
        },
      ],
    };
  },
  components: {
    FooterBot,
  },
};
</script>
<template>
  <section class="bg-image">
    <div class="container">
      <div class="col-1">
        <ul>
          <li>
            <h3>{{ linkFooter1[0].title }}</h3>
          </li>
          <li v-for="li in linkFooter1">
            <a href="{{ li.link }}">{{ li.name }}</a>
          </li>
        </ul>

        <ul>
          <li>
            <h3>{{ linkFooter2[0].title }}</h3>
          </li>
          <li v-for="li in linkFooter2">
            <a href="{{ li.link }}">{{ li.name }}</a>
          </li>
        </ul>
        <ul>
          <li>
            <h3>{{ linkFooter3[0].title }}</h3>
          </li>
          <li v-for="li in linkFooter3">
            <a href="{{ li.link }}">{{ li.name }}</a>
          </li>
        </ul>
        <ul>
          <li>
            <h3>{{ linkFooter4[0].title }}</h3>
          </li>
          <li v-for="li in linkFooter4">
            <a href="{{ li.link }}">{{ li.name }}</a>
          </li>
        </ul>
      </div>
      <img src="../../public/img/dc-logo-bg.png" alt="" />
    </div>
  </section>
  <FooterBot></FooterBot>
</template>
<style scoped lang="scss">
@use '../style/partials' as *;

.bg-image {
  background-image: url(../../public/img/footer-bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: top, right;
  overflow: hidden;

  .container {
    height: 100%;
    align-items: flex-end;
    position: relative;
    .col-1 {
      width: calc(100% / 3);
      flex-wrap: wrap;
      display: flex;
      padding: 30px 0;

      ul {
        margin-right: 30px;

        li {
          color: #959595;
          line-height: 1.6;

          &:hover {
            color: white;
          }

          h3 {
            color: white;
            margin-bottom: 10px;
            text-transform: uppercase;
          }
        }
      }
    }

    img {
      position: absolute;
      right: 0;
      top: -100px;
      width: 630px;
    }
  }
}
</style>
