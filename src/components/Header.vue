<template>
  <div class="header">
    <h3>{{ title1 }}</h3>
    <button @click="changeTitle">Change title</button>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String
    }
  },
  data() {
    return { title1: this.title };
  },
  methods: {
    changeTitle() {
      this.title1 = 'My Changed Title';
    }
  }
};
</script>

<style>
.header {
  display: flex;
  justify-content: center;
  background: chartreuse;
  color: #000;
  font-family: sans-serif;
  letter-spacing: 2.5px;
}
</style>
