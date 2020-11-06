<template>
  <Header></Header>
  <main>
<!--    Home Page Compenent-->
    <Home></Home>

    <!--Profile Page Component-->
<!--        <Profile></Profile>-->
  </main>
  <Footer></Footer>
</template>

<script>
import Header from "@/layouts/Header";
import Footer from "@/layouts/Footer";
import Home from "@/pages/Home";
// import Profile from "@/pages/Profile";

export default {
  name: 'App',
  components: {
    Home,
    // Profile,
    Footer,
    Header,
  }
}
</script>

<style>
@import "./assets/style.css";
</style>
