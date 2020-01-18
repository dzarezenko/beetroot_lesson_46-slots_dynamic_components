<template>
  <div id="quote">
    <header>
      <slot name="quoteTitle">
        <h1>DEFAULT TITLE</h1>
      </slot>
    </header>
    <hr />
    <main>
      <slot name="quoteText" />
    </main>
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