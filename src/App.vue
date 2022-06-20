<script setup>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import MemberGift from "./components/MemberGift";
import Footer from "./components/Footer";
import { ref } from "vue";
</script>

<template lang="">
  <Header />
  <Main />
  <MemberGift v-if="currentIndex == 1" />
  <Footer />
</template>
<style lang=""></style>
