<template>
<section>
  <MobileHeader></MobileHeader>
  <Banner></Banner>
  <Collections></Collections>
  <Testimonials></Testimonials>
  <Contact></Contact>
</section>
</template>

<script>
import Banner from "@/components/home/Banner";
import Collections from "@/components/home/Collections";
import Testimonials from "@/components/home/Testimonials";
import Contact from "@/components/home/Contact";
import MobileHeader from "@/layouts/MobileHeader";
export default {
  name: "Home",
  components: {MobileHeader, Contact, Testimonials, Collections, Banner}
}
</script>

<style scoped>

</style>
