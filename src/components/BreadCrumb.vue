<template>
  <ul class="breadcrumb-list">
    <li class="breadcrumb-item">
      <router-link class="breadcrumb-link" to="/">
        Home
      </router-link>
    </li>
    <li class="breadcrumb-item">/</li>
    <li class="breadcrumb-item">
      <a class="breadcrumb-link" href="#">My Profile</a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "BreadCrumb"
}
</script>

<style scoped>
.breadcrumb-list {
  display: flex;
}

.breadcrumb-item {
  margin-right: 1rem;
}

.breadcrumb-link {
  font-weight: normal;
  font-size: 1.2rem;
  line-height: 1.7px;
  color: #777777;
}
</style>
