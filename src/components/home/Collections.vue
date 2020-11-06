<template>
  <section class="collections">
    <!--Collections Heading-->
    <h2 class="collections-heading"><small>Latest Collections</small></h2>
    <!--Collections Images-->
    <article class="collections-container">
      <!--Image 1-->
      <figure>
        <img class="collections-img" src="../../assets/img/collection1.png">
        <figcaption class="collections-title">Printed Polo T-Shirt</figcaption>
        <h6 class="collections-price">₹1,499.00</h6>
      </figure>
      <!--Image 2-->
      <figure>
        <img class="collections-img" src="../../assets/img/collection2.png">
        <figcaption class="collections-title">Printed Polo T-Shirt</figcaption>
        <h6 class="collections-price">₹1,499.00</h6>
      </figure>
      <!--Image 3-->
      <figure>
        <img class="collections-img" src="../../assets/img/collection1.png">
        <figcaption class="collections-title">Printed Polo T-Shirt</figcaption>
        <h6 class="collections-price">₹1,499.00</h6>
      </figure>
      <!--Image 4-->
      <figure>
        <img class="collections-img" src="../../assets/img/collection2.png">
        <figcaption class="collections-title">Printed Polo T-Shirt</figcaption>
        <h6 class="collections-price">₹1,499.00</h6>
      </figure>
    </article>
  </section>
</template>

<script>
export default {
  name: "Collections"
}
</script>

<style scoped>
.collections {
  padding: 5rem;
}

.collections-heading {
  font-family: "Bank Gothic";
  text-align: center;
  font-size: 2rem;
  color: #333333;
  margin-bottom: 5rem;
  text-transform: uppercase;
  border-bottom: 1px solid #DDDDDD;
  line-height: 0.1rem;
}

.collections-container {
  display: grid;
  grid-column-gap: 2rem;
  grid-template-columns: auto auto auto auto;
}

.collections-heading small {
  background: white;
  padding: 0 1rem;
}

.collections-container {
  text-align: center;
}

small {
  font-size: inherit;
}

.collections-title {
  margin: 1rem 0;
}

.collections-price {
  font-size: 1.3rem;
  line-height: 1.9rem;
  color: #E10000;
  font-weight: normal;
}
</style>
