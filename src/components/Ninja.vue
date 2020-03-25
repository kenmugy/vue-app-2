<template>
  <div class="main">
    <div class="col" v-for="ninja in ninjas" :key="ninja.id">
      <h3>
        {{ ninja.name }} - <span>{{ ninja.id }}</span>
      </h3>
      <h5 v-show="ninja.show">{{ ninja.speciality }}</h5>
      <button @click="ninja.show = !ninja.show">toggle</button>
    </div>
  </div>
</template>

<script>
export default {
  props: ['ninjas'],
  data() {
    return {};
  }
};
</script>

<style>
.main {
  text-align: center;
}
.col {
  display: inline-block;
  width: 25%;
  background: rgb(238, 255, 220);
  margin: 5px;
}
button {
  border: none;
  background: chartreuse;
  padding: 10px;
  margin-bottom: 5px;
  cursor: pointer;
}
button:hover {
  background: #000;
  color: chartreuse;
}
</style>
