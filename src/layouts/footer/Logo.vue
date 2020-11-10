<template>
  <ul class="footer-list__logo">
    <li class="footer-item">
      <router-link to="/">
        <figure>
          <img class="footer-logo" src="./../../assets/img/logo.png">
        </figure>
      </router-link>
    </li>
    <li class="footer-item"><a class="footer-link" href="#">Stay in touch with us</a></li>
    <li class="footer-item">
      <ul class="footer-icon-list">
        <li class="footer-icon-item">
          <a class="footer-icon-link"
             href="#">
            <i class="fa fa-facebook"
               aria-hidden="true">
            </i>
          </a>
        </li>
        <li class="footer-icon-item">
          <a class="footer-icon-link"
             href="#">
            <i class="fa fa-instagram"
               aria-hidden="true">
            </i>
          </a>
        </li>
        <li class="footer-icon-item">
          <a class="footer-icon-link"
             href="#">
            <i class="fa fa-youtube-play"
               aria-hidden="true">
            </i>
          </a>
        </li>
      </ul>
    </li>
  </ul>
</template>

<script>
export default {
  name: "Logo"
}
</script>

<style scoped>
.footer-list__logo {
  text-align: center;
}

.footer-list__logo .footer-icon-item {
  margin: 0 1.5rem;
}

.footer-list__logo .footer-icon-link .fa {
  height: 30px;
  width: 30px;
  background: #BBBBBB;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  font-size: 1.8rem;
  color: #333333;
}

.footer-list__logo .footer-logo {
  height: 7rem;
  width: 10rem;
  object-fit: cover;
}

.footer-list__logo .footer-link {
  color: #DDDDDD;
}
</style>

