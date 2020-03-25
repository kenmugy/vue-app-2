<template>
  <div class="footer">
    <p>{{ copy }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      copy: 'Copyright kenNinja 2002'
    };
  }
};
</script>

<style>
.footer {
  display: flex;
  justify-content: center;
  color: chartreuse;
  background: #000;
  letter-spacing: 1.5px;
}
</style>
