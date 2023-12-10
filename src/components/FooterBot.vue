<script>
export default {
  name: 'FooterBottom',
  data() {
    return {
      socials: [
        {
          name: 'facebook',
          link: '#',
          target: '_self',
          img: '../../public/img/footer-facebook.png',
        },
        {
          name: 'twitter',
          link: '#',
          target: '_self',
          img: '../../public/img/footer-twitter.png',
        },
        {
          name: 'youtube',
          link: '#',
          target: '_self',
          img: '../../public/img/footer-youtube.png',
        },
        {
          name: 'pinterest',
          link: '#',
          target: '_self',
          img: '../../public/img/footer-pinterest.png',
        },
        {
          name: 'periscope',
          link: '#',
          target: '_self',
          img: '../../public/img/footer-periscope.png',
        },
      ],
    };
  },
};
</script>
<template>
  <!-- sezione FooterBOt -->
  <section>
    <!-- container FooterBot di col-1 & col-2 -->
    <div class="container">
      <!-- col-1 -->
      <div class="col-1">
        <button><a href="">Sing-up Now!</a></button>
      </div>
      <!-- col-1 -->

      <!-- col-2 -->
      <div class="col-2">
        <h3>Follow us</h3>
        <!-- lista link -->
        <ul>
          <!-- li con ciclato -->
          <li v-for="li in socials">
            <img :src="li.img" alt="" />
          </li>
        </ul>
        <!-- lista link -->
      </div>
      <!-- col-2 -->
    </div>
    <!-- container FooterBot -->
  </section>
  <!-- sezione FooterBOt -->
</template>
<style scoped lang="scss">
@use '../style/partials' as *;

section {
  background-color: #303030;
  padding: 30px 0;

  button {
    padding: 15px 30px;
    border: 2px solid #0282f9;
    text-transform: uppercase;
    color: white;
    font-weight: bolder;
  }

  .col-2 {
    display: flex;
    align-items: center;
    gap: 30px;

    h3 {
      color: #0282f9;
      text-transform: uppercase;
    }

    ul {
      display: flex;
      gap: 20px;
    }
  }
}
</style>
