<script>
export default {
  nome: 'header',
  data() {
    return {
      links: [
        {
          name: 'characters',
          link: '#',
          target: '_self',
        },
        {
          name: 'Comics',
          link: '#',
          target: '_self',
        },
        {
          name: 'movies',
          link: '#',
          target: '_self',
        },
        {
          name: 'tv',
          link: '#',
          target: '_self',
        },
        {
          name: 'Games',
          link: '#',
          target: '_self',
        },
        {
          name: 'collectibles',
          link: '#',
          target: '_self',
        },
        {
          name: 'videos',
          link: '#',
          target: '_self',
        },
        {
          name: 'fans',
          link: '#',
          target: '_self',
        },
        {
          name: 'news',
          link: '#',
          target: '_self',
        },
        {
          name: 'shop',
          link: '#',
          target: '_self',
        },
      ],
    };
  },
};
</script>

<template>
  <!-- container Header -->
  <div class="container">
    <img src="../../public/img/dc-logo.png" alt="" />

    <!-- lista link -->
    <ul>
      <!-- li ciclato -->
      <li v-for="li in links">
        <a href="#">{{ li.name }}</a>
      </li>
    </ul>
    <!-- lista link -->
  </div>
  <!-- container Header -->
</template>

<style scoped lang="scss">
@use '../style/partials' as *;
@use '../style/variables' as *;
.container {
  img {
    width: 70px;
  }
  ul {
    list-style: none;
    display: flex;
    text-transform: uppercase;
    font-size: 12px;
    font-weight: bolder;
    gap: 20px;
  }

  li {
    height: 90px;
    display: flex;
    align-items: center;
    cursor: pointer;

    &:hover {
      border-bottom: 4px solid #0282f9;
      color: #0282f9;
    }
  }
}
</style>
