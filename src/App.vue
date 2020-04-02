<template>
  <div class="app">
    <Header :title="title" @changeTitle="updateTitle($event)" />
    <Ninja :ninjas="ninjas" />
    <Footer :title="title" />
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
  },
  data() {
    return {
      ninjas: [
        {
          id: 0,
          name: 'Ryu',
          speciality: 'React & Vue',
          show: false
        },
        {
          id: 1,
          name: 'Mario',
          speciality: 'Angular & jquery',
          show: false
        },
        {
          id: 2,
          name: 'Ryu',
          speciality: 'Svelte',
          show: false
        }
      ],
      title: 'My new title'
    };
  },
  methods: {
    updateTitle(val) {
      this.title = val;
    }
  }
};
</script>
