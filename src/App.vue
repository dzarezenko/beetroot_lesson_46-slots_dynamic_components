<template>
  <div id="app">
    <Quote>
      <h1 slot="quoteTitle">{{ quoteTitleVal }}</h1>
      <p slot="quoteText">{{ quoteTextVal }}</p>
    </Quote>
    <br />

    <my-link url="http://google.com"><i class="fa fa-user" /> Link Text</my-link>

  </div>
</template>

<script>
import Quote from "@/components/Quote";
import MyLink from "@/components/MyLink";

export default {
  data() {
    return {
      quoteTitleVal: "Some title",
      quoteTextVal: "Some long text",
    }
  },
  components: {
    Quote,
    myLink: MyLink,
  },
}
</script>
