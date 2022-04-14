<template>
  <div>
    <app-header></app-header>
    <div class="container">
      <compUserProfile :alsoKnownAs="name" lastname="Gowen"></compUserProfile>
      <button @click="updateName">Update name</button>
    </div>

    <app-footer></app-footer>
  </div>
</template>

<script>
import compUserProfile from "./components/user/Profile.vue";
export default {
  components: {
    compUserProfile,
  },
  data() {
    return {
      name: "Clonie",
    };
  },
  methods: {
    updateName() {
      this.name = "Mike";
    },
  },
};
</script>

<style>
body {
  padding: 0;
  margin: 0;
  font-family: "Roboto", sans-serif;
}

.container {
  min-height: 84vh;
  box-sizing: border-box;
  padding: 20px;
}
</style>
