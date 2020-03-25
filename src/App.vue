<template>
  <div class="app">
    <Header />
    <Ninja />
    <Footer />
  </div>
</template>
<script>
import Header from './components/Header';
import Ninja from './components/Ninja';
import Footer from './components/Footer';
export default {
  components: {
    Header,
    Ninja,
    Footer
  }
};
</script>
