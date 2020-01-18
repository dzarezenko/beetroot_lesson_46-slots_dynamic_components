<template>
  <div id="app">
    <button @click="currentComponent = 'UserPhoto'">User Photo</button> |
    <button @click="currentComponent = 'UserContacts'">User Contacts</button> |
    <button @click="currentComponent = 'UserDetails'">User Details</button>
    <p>
      {{ currentComponent }}
    </p>
    <hr />

    <component :is="currentComponent"></component>

  </div>
</template>

<script>
import UserPhoto from "@/components/user/UserPhoto";
import UserContacts from "@/components/user/UserContacts";
import UserDetails from "@/components/user/UserDetails";

export default {
  data() {
    return {
      currentComponent: "UserPhoto",
    }
  },
  components: {
    UserPhoto, UserContacts, UserDetails
  },
}
</script>
