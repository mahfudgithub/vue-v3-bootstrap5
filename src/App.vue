<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-success shadow-sm my-1">
    <div class="container">
      <label class="navbar-brand">Vue App</label>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <RouterLink class="nav-link" aria-current="page" to="/">Home</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link" :to="{ name: 'aboutpath' }">About</RouterLink>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <RouterView />
</template>

<style></style>
