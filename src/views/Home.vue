<template>
  <div>
    <Navbar/>
    <Videobar/>
    <Inplay/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue';
import Videobar from '@/components/Videobar.vue';
import Inplay from '@/pages/Inplay.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'Home',
  components: {
    Navbar,
    Videobar,
    Inplay,
    Footer,
  }
}
</script>
