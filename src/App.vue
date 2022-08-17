<template>
  <div>
    <HeaderItem :links="headerMenu" />
    <MainItem :gallery="dcComicsData" />
    <FooterItem />
  </div>
</template>

<script>
import HeaderItem from './components/HeaderItem.vue';
import MainItem from './components/MainItem.vue';
import FooterItem from './components/FooterItem.vue';
import json from './assets/js/dc-comics.json';
export default {
  name: 'DcComics',
  components: {
    HeaderItem,
    MainItem,
    FooterItem,
  },
  data() {
    return {
      headerMenu:[
        {id:1, url:'#', text:'CHARACTERS', active: false},
        {id:2, url:'#', text:'COMICS', active: false},
        {id:3, url:'#', text:'MOVIES', active: false},
        {id:4, url:'#', text:'TV', active: false},
        {id:5, url:'#', text:'GAMES', active: false},
        {id:6, url:'#', text:'COLLECTIBLES', active: false},
        {id:7, url:'#', text:'VIDEOS', active: false},
        {id:8, url:'#', text:'FANS', active: false},
        {id:9, url:'#', text:'NEWS', active: false},
        {id:10, url:'#', text:'SHOP', active: false},
      ],
      dcComicsData: json,
    }
  },
};
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
    background-color: black;
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
