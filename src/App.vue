<template>
  <div>
    <HeaderItem :links="headerMenu" />
    <MainItem :gallery="dcComicsData" :bannerMenu="bannerMenu" />
    <FooterItem 
    :footerDcComicsMenu="footerDcComicsMenu"
    :footerShopMenu="footerShopMenu"
    :footerDcMenu="footerDcMenu"
    :footerSitesMenu="footerSitesMenu"
    :footerSocialMenu="footerSocialMenu"
    />
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
      bannerMenu:[
        {id:1, 
        src: require('./assets/img/buy-comics-digital-comics.png'), 
        text: 'DIGITAL COMICS', url: '#'
        },
        {id:1, 
        src: require('./assets/img/buy-comics-merchandise.png'), 
        text: 'DC MERCHANDISE', url: '#'
        },
        {id:1, 
        src: require('./assets/img/buy-comics-subscriptions.png'), 
        text: 'SUBSCRIPTION', url: '#'
        },
        {id:1, 
        src: require('./assets/img/buy-comics-shop-locator.png'), 
        text: 'SHOP LOCATOR', url: '#'
        },
        {id:1, 
        src: require('./assets/img/buy-dc-power-visa.svg'), 
        text: 'DC POWER VISA', url: '#'
        },
      ],
      footerDcComicsMenu: [
        {id:1, url:'#', text:'Characters'},
        {id:2, url:'#', text:'Comics'},
        {id:3, url:'#', text:'Movies'},
        {id:4, url:'#', text:'TV'},
        {id:5, url:'#', text:'Games'},
        {id:6, url:'#', text:'Videos'},
        {id:7, url:'#', text:'News'},
      ],
      footerShopMenu: [
        {id:1, url:'#', text:'Shop DC'},
        {id:2, url:'#', text:'Shop DC Collectibles'},
      ],
      footerDcMenu: [
        {id:1, url:'#', text:'Terms Of Use'},
        {id:2, url:'#', text:'Privacy policy (New)'},
        {id:3, url:'#', text:'Ad Choices'},
        {id:4, url:'#', text:'Advertising'},
        {id:5, url:'#', text:'Jobs'},
        {id:6, url:'#', text:'Subscriptions'},
        {id:7, url:'#', text:'Talent Workshops'},
        {id:8, url:'#', text:'CPSC Certificates'},
        {id:9, url:'#', text:'Ratings'},
        {id:10, url:'#', text:'Shop Help'},
        {id:11, url:'#', text:'Contact Us'},
      ],
      footerSitesMenu: [
        {id:1, url:'#', text:'DC'},
        {id:2, url:'#', text:'MAD Magazine'},
        {id:3, url:'#', text:'DC Kids'},
        {id:4, url:'#', text:'DC Universe'},
        {id:5, url:'#', text:'DC Power Visa'},
      ],
      footerSocialMenu: [
        {id:1, 
        url: '#', 
        src: require('./assets/img/footer-facebook.png'), 
        text: 'Facebook logo'
        },
        {id:2, 
        url: '#', 
        src: require('./assets/img/footer-twitter.png'), 
        text: 'Twitter logo'
        },
        {id:3, 
        url: '#', 
        src: require('./assets/img/footer-youtube.png'), 
        text: 'Youtube logo'
        },
        {id:4, 
        url: '#', 
        src: require('./assets/img/footer-pinterest.png'), 
        text: 'Pinterest logo'
        },
        {id:5, 
        url: '#', 
        src: require('./assets/img/footer-periscope.png'), 
        text: 'Periscope logo'
        },
      ],
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
