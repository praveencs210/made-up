<template>
  <section class="contact">
    <article class="contact-container">
      <article>
        <h2 class="contact-title">GET COUPONS & STYLE GUIDES</h2>
        <h6 class="contact__sub-title">Subscribe to our Newsletter</h6>
      </article>
      <form>
        <fieldset class="contact-fieldset">
          <input class="contact-email" type="text" placeholder="E-mail ID">
          <button class="btn-subscribe" type="submit">SUBSCRIBE</button>
        </fieldset>
      </form>
      <button type="submit" class="btn-location">
        <i class="fa fa-map-marker" aria-hidden="true"></i> LOCATE US
      </button>
    </article>
  </section>
</template>

<script>
export default {
  name: "Contact"
}
</script>

<style scoped>
.contact {
  line-height: 0;
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), url('../../assets/img/contact.png');
  background-repeat: no-repeat;
  background-position: top center;
  background-size: cover;
  padding: 10rem 0;
  text-align: center;
  width: 100%;
  height: 36rem;
  position: relative;
}

.contact-title {
  font-weight: 600;
  font-size: 24px;
  line-height: 35px;
  color: #FFFFFF;
}

.contact__sub-title {
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 29px;
  color: #FFFFFF;
  margin: 2rem 0;
}

input{
  border: 0;
  background: white;
  color: #DEDEDE;
  height: 4rem;
  border-radius: 0.3rem;
  width: 30%;
  margin-right: 1rem;
  padding: 0 1rem;
}

.btn-subscribe{
  background: #E10000;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 20px;
  height: 4rem;
  color: #FFFFFF;
  padding: 0 2rem;
  border: 1px solid #E10000;
}

.btn-location{
  position: absolute;
  right: 10%;
  bottom: 0;
  background: #222222;
  box-shadow: 6px 0px 20px rgba(0, 0, 0, 0.25);
  border-radius: 6px 6px 0px 0px;
  border: 0;
  height: 40px;
  padding: 0 2rem;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 23px;
  color: #DDDDDD;
}

.btn-location .fa{
  margin-right: 1rem;
}
</style>
