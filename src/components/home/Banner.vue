<template>
  <section class="banner">
    <!--    Home Page Banner-->
    <article class="banner-container">
      <figure class="banner-img"></figure>
      <hgroup class="banner-content">
        <h6 class="banner-text"> Clothes that <p class="banner__text-highlight">respire</p></h6>
        <h6 class="banner-text"> for men who <p class="banner__text-highlight">aspire</p></h6>
      </hgroup>
      <button type="submit"
              class="btn-browse">
        BROWSE COLLECTIONS
      </button>
    </article>
    <!--    Home Page Banner Grid Images-->
    <article class="grid-container">
      <figure class="grid-items">
        <img src="../../assets/img/banner2.png">
        <hgroup class="banner-content">
          <h6 class="banner-text"><p class="banner__text-highlight">Summer</p> is here and</h6>
          <h6 class="banner-text"> so is our<p class="banner__text-highlight">collection</p></h6>
        </hgroup>
      </figure>

      <ul class="grid-column">
        <li>
          <figure class="grid-items">
            <img src="../../assets/img/banner3.png">
            <hgroup class="banner-content">
              <h6 class="banner-text"><p class="banner__text-highlight">Wrinkle-free</p> t-shirts</h6>
            </hgroup>
          </figure>
        </li>

        <li>
          <figure class="grid-items">
            <img src="../../assets/img/banner4.png">
            <hgroup class="banner-content">
              <h6 class="banner-text"><p class="banner__text-highlight">Stain-free</p> denim shirts</h6>
            </hgroup>
          </figure>
        </li>
      </ul>
    </article>
  </section>
</template>

<script>
export default {
  name: "Banner"
}
</script>

<style scoped>
.banner-img {
  margin-bottom: 1rem;
  background-image: url("../../assets/img/banner1.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: top center;
  height: 93vh;
}

.banner-container,
.grid-items {
  position: relative;
}

.banner-content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.banner-text {
  display: flex;
  justify-content: center;
  align-items: center;
  background: var(--white);
  font-style: normal;
  font-weight: normal;
  font-size: 2rem;
  line-height: 2.9rem;
  color: #333333;
  margin-bottom: 1rem;
  padding: 0 1rem;
  white-space: pre;
}

.banner__text-highlight {
  margin-left: 1rem;
  color: var(--primary);
}

.btn-browse {
  position: absolute;
  top: 70%;
  left: 50%;
  transform: translate(-50%, -50%);
  background: #E10000;
  font-style: normal;
  font-weight: 500;
  font-size: 1.6rem;
  line-height: 2.3rem;
  height: 5rem;
  color: #FFFFFF;
  padding: 0 3rem;
  border: 1px solid #E10000;
}

.grid-container {
  display: grid;
  grid-column-gap: 1rem;
  grid-row-gap: 10rem;
  grid-template-columns: auto auto auto;
}

.grid-column li:nth-child(1) {
  margin-bottom: 0.5rem;
}
</style>
