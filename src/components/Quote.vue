<template>
  <div id="quote">
    <slot />
  </div>
</template>

<script>
export default {
  props: ["quote"],
}
</script>

<style scoped>
#quote {
  width: 100%;
  text-align: center;
  background-color: #ccc;
  border: 1px solid #000;
  padding: 20px 0px;
}
</style>