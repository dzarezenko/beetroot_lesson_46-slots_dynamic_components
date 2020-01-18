<template>
  <div>
    <h1>User Contacts</h1>
    <button @click="counter++">+</button>
    <p>Counter: {{ counter }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      counter: 0,
    }
  },
  destroyed() {
    console.log("Component destroyed!");
  },
  activated() {
    console.log("Activated!");
  },
  deactivated() {
    console.log("Deactivated!");
  },
}
</script>
