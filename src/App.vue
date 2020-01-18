<template>
  <div id="app">
    <Quote>
      <template #quoteTitle>
        <h1>{{ quoteTitleVal }}</h1>
      </template>
      <template #quoteText>
        <p>{{ quoteTextVal }}</p>
      </template>
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
