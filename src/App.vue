<template>
  <Navbar :logo="logo_src" :alt="app_name"/>
  <router-view/>
  <FooterMain/>
</template>

<style lang="scss">

</style>
<script lang="ts">
import Navbar from '@/components/Navbar.vue';
import FooterMain from '@/components/Footer.vue';

export default {
  data() {
    return {
      // eslint-disable-next-line global-require
      logo_src: '/img/logo.png',
      app_name: 'Make Your Burger'
    };
  },
  components: {
    FooterMain,
    Navbar,
  }
};
</script>

<style>
* {
  font-family: Helvetica, serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
