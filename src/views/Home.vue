<template>
  <div>
    <Banner />
    <div class="main-container">
      <h1>Monte seu burger:</h1>
      <p>formulário</p>
    </div>
  </div>
</template>

<script lang="ts">
import Banner from "../components/Banner.vue";
export default {
  name: "Home",
  components: {
    Banner,
  },
};
</script>
