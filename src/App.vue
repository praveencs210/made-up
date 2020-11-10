<template>
  <Header></Header>
  <main>
    <router-view/>
  </main>
  <Footer></Footer>
</template>

<style>
@import "assets/style.css";
</style>

<script>
import Header from "@/layouts/Header";
import Footer from "@/layouts/Footer";

export default {
  components: {Footer, Header}
}
</script>
