<template>
  <section class="mobile-header">
    <a href="#"><i class="fa fa-chevron-left" aria-hidden="true"></i></a>
    <router-link to="/my-profile" class="mobile-header__container">
      <img class="mobile-header__img active" src="../assets/img/category/category1.png">
      <figcaption class="mobile-header__title">For Me</figcaption>
    </router-link>
    <a href="#" class="mobile-header__container">
      <img class="mobile-header__img" src="../assets/img/category/category2.png">
      <figcaption class="mobile-header__title">Jeans</figcaption>
    </a>
    <a href="#" class="mobile-header__container">
      <img class="mobile-header__img" src="../assets/img/category/category3.png">
      <figcaption class="mobile-header__title">T-Shirts</figcaption>
    </a>
    <a href="#" class="mobile-header__container">
      <img class="mobile-header__img" src="../assets/img/category/category4.png">
      <figcaption class="mobile-header__title">Shirts</figcaption>
    </a>
    <a href="#" class="mobile-header__container">
      <img class="mobile-header__img" src="../assets/img/category/category5.png">
      <figcaption class="mobile-header__title">Trousers</figcaption>
    </a>
    <a href="#"><i class="fa fa-chevron-right" aria-hidden="true"></i></a>
  </section>
</template>

<script>
export default {
  name: "MobileHeader"
}
</script>
