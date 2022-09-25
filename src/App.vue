<template>
  <body class="body">
    <Header :logo="logo_src" :alt="app_name" />
    <Footer />
  </body>
</template>

<script lang="ts">
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Header,
    Footer,
  },
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Make Your Burger",
    };
  },
};
</script>

<style>
body {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
}

.body {
  background-color: #ffffff;
  color: #222;
}

.main-container {
  margin: 50px;
  min-height: 250px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
