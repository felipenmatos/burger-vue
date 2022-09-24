<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">
          <img :src="logo" :alt="alt" id="logo" />
        </RouterLink>
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
