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
  <section>
    <div class="container">
      <div class="col-1">
        <button><a href="">Sing-up Now!</a></button>
      </div>
      <div class="col-2">
        <h3>Follow us</h3>
        <ul>
          <li v-for="li in socials">
            <img :src="li.img" alt="" />
          </li>
        </ul>
      </div>
    </div>
  </section>
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
