<template>
  <div class="header">
    <h3>{{ title }}</h3>
    <button @click="changeTitle">Change title</button>
  </div>
</template>

<script>
export default {
  props: ['title'],
  data() {
    // return { title1: this.title };
  },
  methods: {
    changeTitle() {
      this.$emit('changeTitle', 'My Changed Title');
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
