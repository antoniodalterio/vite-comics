<script>
export default {
  name: 'contentMain',
  data() {
    return {
      nav: [
        {
          name: 'digital comics',
          link: '#',
          target: '_self',
          img: '../../public/img/buy-comics-digital-comics.png',
        },
        {
          name: 'dc merchandise',
          link: '#',
          target: '_self',
          img: '../../public/img/buy-comics-merchandise.png',
        },
        {
          name: 'subcription',
          link: '#',
          target: '_self',
          img: 'public/img/buy-comics-subscriptions.png',
        },
        {
          name: 'comic shop',
          link: '#',
          target: '_self',
          img: 'public/img/buy-comics-shop-locator.png',
        },
        {
          name: 'dc Power visa',
          link: '#',
          target: '_self',
          img: 'public/img/buy-dc-power-visa.svg',
        },
      ],
    };
  },
};
</script>
<template>
  <!-- sezione navbar -->
  <section>
    <!-- contenitore -->
    <div class="container">
      <!-- lista link nav -->
      <ul>
        <li v-for="li in nav">
          <!-- imagine nav -->
          <img :src="li.img" alt="" />
          <!-- link -->
          <a href="{{li.link}}" target="{{li.target}}">
            <p>{{ li.name }}</p></a
          >
        </li>
      </ul>
      <!-- lista link nav -->
    </div>
    <!-- contenitore -->
  </section>
  <!-- sezione navbar -->
</template>
<style scoped lang="scss">
@use '../style/partials' as *;
@use '../style/variables' as *;
section {
  padding: 50px;
  background-color: #0282f9;

  .container {
    ul {
      display: flex;
      height: 100%;
      gap: 70px;

      li {
        display: flex;
        align-items: center;
        gap: 15px;

        img {
          width: 45px;
          height: 60px;
        }

        p {
          color: white;
          text-transform: uppercase;
        }
      }
    }
  }
}
</style>
