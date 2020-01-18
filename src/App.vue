<template>
  <div id="app">
    <Quote>
      <h1 slot="quoteTitle">{{ quoteTitleVal }}</h1>
      <p slot="quoteText">{{ quoteTextVal }}</p>
    </Quote>
  </div>
</template>

<script>
import Quote from "@/components/Quote";

export default {
  data() {
    return {
      quoteTitleVal: "Some title",
      quoteTextVal: "Some long text",
    }
  },
  components: {
    Quote,
  },
}
</script>
