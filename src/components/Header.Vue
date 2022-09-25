<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div class="wrapper">
      <RouterLink to="/">
        <img :src="logo" :alt="alt" id="logo" />
      </RouterLink>
      <nav id="nav">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/pedidos">Pedidos</RouterLink>
      </nav>
    </div>
  </header>
  <RouterView />
</template>

<script lang="ts">
export default {
  props: ["logo", "alt"],
};
</script>

<style>
.wrapper {
  max-width: 100%;
  width: 100vw;
  background-color: #222;
  border-bottom: 4px solid #111;
  padding: 15px 50px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header {
  width: 100%;
  display: flex;
  background: red;
}

img {
  width: 50px;
  height: 50px;
}

#nav a {
  color: #fcba03;
  text-decoration: none;
  margin: 12px;
  transition: 0.5s;
}

#nav a:hover {
  color: #fff;
}
</style>
