<template>
  <header class="header">
    <!--Logo-->
    <a href="#" class="logo">
      <h1 class="logo-heading">
        Made Up
      </h1>
    </a>

    <!--Nav Link-->
    <ul class="nav-list header-nav-none">
      <li class="nav-item"><a class="nav-link active" href="#">For Me</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Jeans</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Shirts</a></li>
      <li class="nav-item"><a class="nav-link" href="#">T-Shirts</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Trousers</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Joggers</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Shorts</a></li>
    </ul>

    <!--Nav Icon-->
    <nav class="nav">
      <ul class="nav-list">
        <li class="nav-item"><a class="nav-link" href="#"><i class="icon icon-Path-16"></i></a></li>
        <li class="nav-item"><a class="nav-link" href="#"><i class="icon icon-Path-19"></i></a></li>
        <li class="nav-item d-md-none"><a class="nav-link" href="#"><i class="icon icon-Path-35"></i></a></li>
        <li class="nav-item d-md-none"><a class="nav-link" href="#"><i class="icon icon-Path-41"></i></a></li>

        <li class="nav-item">
          <ul>
            <li class="nav-item">
              <nav class=" d-lg-none">
                <a href="#main-menu"
                   id="main-menu-toggle"
                   class="menu-toggle"
                   aria-label="Open main menu">
                  <i class="sr-only">Open main menu</i>
                  <span class="fa fa-bars" aria-hidden="true"></span>
                </a>

                <nav id="main-menu" class="main-menu" aria-label="Main menu">
                  <a href="#main-menu-toggle"
                     id="main-menu-close"
                     class="menu-close"
                     aria-label="Close main menu">
                    <i class="sr-only">Close main menu</i>
                    <i class="fa fa-close" aria-hidden="true"></i>
                  </a>

                  <h2 id="main-menu-heading" class="sr-only">Main menu</h2>
                  <ul class="hamburger-list" aria-labelledby="main-menu-heading">
                    <li class="hamburger-item"><a class="hamburger-link active" href="#">My Profile</a></li>
                    <li class="hamburger-item"><a class="hamburger-link " href="#"> My Wishlist</a></li>
                    <li class="hamburger-item"><a class="hamburger-link " href="#">My Orders</a></li>
                    <li class="hamburger-item"><a class="hamburger-link " href="#">My Addresses</a></li>
                    <hr/>
                    <li class="hamburger-item"><a class="hamburger-link active" href="#">The Brand</a></li>
                    <li class="hamburger-item"><a class="hamburger-link " href="#">The made up Story </a></li>
                    <li class="hamburger-item"><a class="hamburger-link " href="#">Franchise and Supplieds</a></li>
                    <li class="hamburger-item"><a class="hamburger-link " href="#">Store Locator</a></li>
                  </ul>
                </nav>

                <a href="#main-menu-toggle"
                   class="backdrop"
                   tabindex="-1"
                   aria-hidden="true" hidden></a>
              </nav>
            </li>
          </ul>
        </li>
      </ul>


    </nav>

    <!--Hamburger Menu-->
  </header>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 7rem;
  padding: 0 4rem;
  border-bottom: 1px solid #DDDDDD;
}

.logo {
  height: 7rem;
  width: 10rem;
  background: var(--primary);
}

.logo-heading {
  font-family: 'Scada', sans-serif;
  font-weight: bold;
  font-size: 2rem;
  line-height: 2.5rem;
  text-align: center;
  color: var(--white);
  padding-top: 1rem;
  text-transform: uppercase;
  white-space: pre;
}

.nav-list {
  display: flex;
  align-items: center;
}

.nav-link {
  color: #444444;
  padding: 2.5rem 2rem;
}

.nav-link.active,
.nav-link:hover {
  color: var(--primary);
}

.icon {
  font-size: 1.6rem;
}
</style>
