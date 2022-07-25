<template>
  <div>
    <HeaderItem />
    <MainItem />
    <FooterItem />
  </div>
</template>

<script>
import HeaderItem from './components/HeaderItem.vue';
import MainItem from './components/MainItem.vue';
import FooterItem from './components/FooterItem.vue';
export default {
  name: 'DcComics',
  components: {
    HeaderItem,
    MainItem,
    FooterItem,
  },
}
</script>

<style>
/* Generics */
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    min-height: 100vh;
    background-color: black;
    padding: 50px 0;
  }

  img {
    max-width: 100%;
    height: 60px;
  }

  ul {
    list-style-type: none;
  }

  a {
    color: black;
    text-decoration: none;
  }

  .container {
    margin: 0 auto;
    max-width: 1300px;
  }
</style>
