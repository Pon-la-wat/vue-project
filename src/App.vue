<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue'
import SectionOne from './components/Section_one.vue'
import SectionTwo from './components/Section_two.vue'
import SectionTree from './components/Section_tree.vue'
import SectionFour from './components/Section_four.vue'
</script>

<template>
  <Navbar />
  <SectionOne />
  <SectionTwo />
  <SectionTree />
  <SectionFour />
</template>

<style>
#app {
  position: absolute;
  width: 100%;
  height: 1918px;
  left: 0px;
  top: 0px;
  color: white;
  background: linear-gradient(180deg, #333333 0%, #000000 0.01%);
}
.color-highlight {
    color: #D9EF0C;
}
</style>