<template>
  <div id="app">
    <Quote :quote="quote">

    </Quote>
  </div>
</template>

<script>
import Quote from "@/components/Quote";

export default {
  data() {
    return {
      quote: "<h1>Some title</h1><p>Some long text</p>",
    }
  },
  components: {
    Quote,
  },
}
</script>
