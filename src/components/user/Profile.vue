<template>
  <div class="user_profile">
    <h3>User Information</h3>
    <ul>
      <li><span>Name:</span>{{ name }}</li>
      <li><span>Known as:</span>{{ alsoKnownAs }}</li>
      <li><span>Lastname:</span>{{ lastname }}</li>
    </ul>
  </div>
</template>

<script>
// import { defineComponent } from "@vue/composition-api";

export default {
  props: ["alsoKnownAs", "lastname"],
  data() {
    return {
      name: "Cycalona",
    };
  },
};
</script>

<style scoped>
span {
  font-weight: 800;
  padding: 1px;
}

.user_profile {
  border: 1px solid #2196f3;
  padding: 10px;
}
</style>
