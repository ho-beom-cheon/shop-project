<template>
  <div id="app">
    <Header />
    <router-view />
    <Footer />
  </div>
</template>
<script>
  import Header from '@/components/Header.vue';
  import Footer from '@/components/Footer.vue';

  export default {
    mounted() {
      $.initialize();
    },
    components: {
      Header,
      Footer
    }
  }
</script>