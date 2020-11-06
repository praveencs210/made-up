<template>
  <footer class="footer">
    <!--Footer Link-->
    <Link/>

    <!--Footer Logo-->
    <Logo></Logo>

    <!--Footer Address-->
    <Address></Address>
  </footer>
</template>

<script>
import Link from "@/layouts/footer/Link";
import Logo from "@/layouts/footer/Logo";
import Address from "@/layouts/footer/Address";

export default {
  name: "Footer",
  components: {Address, Logo, Link}
}
</script>

<style>
.footer {
  background: #333333;
  display: flex;
  justify-content: space-around;
  padding: 7rem 0;
}

.footer-item {
  margin: 2rem 0;
}

.footer-link {
  line-height: 2.4rem;
  color: #BBBBBB;
  padding: 2rem 0;
}

.footer-icon-list {
  display: flex;
}
</style>
