<template>
  <section class="testimonials">
    <!--Testimonials Card Heading-->
    <h2 class="testimonials-heading"><small>Testimonials</small></h2>
    <article class="testimonials-container">
      <!--Testimonials Card 1-->
      <figure class="testimonials-card">
        <img class="testimonials-img" src="../../assets/img/testimonials.png">
        <h6 class="testimonials-name">
          Vikas
          <p>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
          </p>
        </h6>
        <p class="testimonials-description">
          Love the cloth material! So breezy and comfortable. Really durable as well. I must say the jeans I bought was
          worth the price.
        </p>
      </figure>
      <!--Testimonials Card 2-->
      <figure class="testimonials-card d-sm-none">
        <img class="testimonials-img" src="../../assets/img/testimonials.png">
        <h6 class="testimonials-name">
          Vikas
          <p>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
          </p>
        </h6>
        <p class="testimonials-description">
          Love the cloth material! So breezy and comfortable. Really durable as well. I must say the jeans I bought was
          worth the price.
        </p>
      </figure>
      <!--Testimonials Card 3-->
      <figure class="testimonials-card d-sm-none d-md-none">
        <img class="testimonials-img" src="../../assets/img/testimonials.png">
        <h6 class="testimonials-name">
          Vikas
          <p>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
            <i class="testimonials-star"></i>
          </p>
        </h6>
        <p class="testimonials-description">
          Love the cloth material! So breezy and comfortable. Really durable as well. I must say the jeans I bought was
          worth the price.
        </p>
      </figure>
    </article>
  </section>
</template>

<script>
export default {
  name: "Testimonials"
}
</script>

<style scoped>
.testimonials {
  background: #F9F9F9;
  padding: 6rem 5rem;
  padding-bottom: 7rem;
}

.testimonials-heading {
  font-family: "Bank Gothic";
  text-align: center;
  font-weight: normal;
  font-size: 2.4rem;
  line-height: 2.5rem;
  color: #333333;
  text-transform: uppercase;
  margin-bottom: 4rem;
}

.testimonials-container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-gap: 10rem;
}

.testimonials-card {
  position: relative;
  background: #FFFFFF;
  box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.08);
  border-radius: 6px;
  padding: 2.5rem;
}

.testimonials-img {
  height: 5rem;
  width: 5rem;
  position: absolute;
  top: -2rem;
  left: -2rem;
}

.testimonials-name {
  display: flex;
  justify-content: space-between;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 20px;
  margin-bottom: 1rem;
  color: #404040;
}

.testimonials-description {
  font-style: italic;
  color: #707070;
}

.testimonials-star {
  position: relative;
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 1rem;
  margin-right: 1.5rem;
  margin-bottom: 1rem;
  border-right: 0.3rem solid transparent;
  border-bottom: 0.7em solid #FDC02F;
  border-left: 0.3em solid transparent;
  font-size: 1rem;
}

.testimonials-star:before, .testimonials-star:after {
  content: "";
  display: block;
  width: 0;
  height: 0;
  position: absolute;
  top: 0.6em;
  left: -1em;
  border-right: 1em solid transparent;
  border-bottom: 0.7em solid #FDC02F;
  border-left: 1em solid transparent;
  -webkit-transform: rotate(-35deg);
  transform: rotate(-35deg);
}

.testimonials-star:after {
  -webkit-transform: rotate(35deg);
  transform: rotate(35deg);
}

</style>
