<template>
  <ul class="footer-list__address">
    <li class="footer-item">
      <p class="footer-link__title">Our Corporate Office</p>
    </li>
    <li class="footer-item">
      <p class="footer-link">
        No: 7,A2B road, Adayar Rajpuram, <br/> T-Nagar, Chennai - 642002.
      </p>
    </li>
    <li class="footer-item__email">
      <a class="footer-link"
         href="mailto:sales@derbymen.com">
        <i class="fa fa-envelope-o" aria-hidden="true"></i>
        sales@derbymen.com
      </a>
    </li>
    <li class="footer-item__phone">
      <a class="footer-link"
         href="tel:044 5566 6889">
        <i class="fa fa-phone" aria-hidden="true"></i>
        044 5566 6889
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "Address"
}
</script>

<style scoped>
.footer-list__address i {
  margin-right: 1rem;
}

.footer-list__address .footer-link__title {
  color: #DDDDDD;
}

.footer-list__address .footer-link {
  padding: 0;
}

.footer-list__address .footer-item__email {
  margin-top: 4rem;
}

.footer-list__address .footer-item__phone {
  margin-top: 1rem;
}

.footer-item__email .footer-link,
.footer-item__phone .footer-link {
  line-height: 2rem;
}
</style>
