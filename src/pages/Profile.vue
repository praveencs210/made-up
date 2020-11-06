<template>
  <section class="section-profile">
    <BreadCrumb></BreadCrumb>
    <Tabs></Tabs>
  </section>
</template>

<script>
import BreadCrumb from "@/components/BreadCrumb";
import Tabs from "@/components/profile/Tabs";

export default {
  name: "Profile",
  components: {Tabs, BreadCrumb},
}
</script>

<style scoped>
.section-profile {
  margin: 4.5rem;
}
</style>
