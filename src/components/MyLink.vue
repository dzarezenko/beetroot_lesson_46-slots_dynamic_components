<template>
  <a :href="url"><slot /></a>
</template>

<script>
export default {
  props: {
    url: {
      type: String,
      required: true,
    },
  },
}
</script>
