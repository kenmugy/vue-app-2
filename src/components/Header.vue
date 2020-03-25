<template>
  <div class="header">
    <h3>{{ title }}</h3>
  </div>
</template>

<script>
export default {
  data() {
    return { title: 'My Ninjaz' };
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
