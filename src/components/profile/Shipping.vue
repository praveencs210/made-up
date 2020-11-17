<template>
  <section class="tab-item" id="section4">
    <input type="radio" name="sections" id="option3">
    <label for="option3">
      <h1 class="tab-title">Shipping Addresses</h1>
      <p class="tab__sub-title">3 ddresses</p>
    </label>
    <article class="tab-content">
      <h1 class="tab-heading">Shipping Address</h1>
      <section class="tab-profile">
        <form>
          <p class="username">
            <input type="text" placeholder="First Name">
            <input type="text" placeholder="Last Name">
          </p>
          <p>
            <input type="text" placeholder="Last Name">
          </p>
          <p>
            <input type="text" placeholder="Email">
          </p>
          <p>
            <input type="text" placeholder="Phone number">
          </p>
          <button class="submit" type="submit">
            Save Changes
          </button>
        </form>
      </section>
    </article>
  </section>
</template>

<script>
export default {
  name: "Shipping"
}
</script>

<style scoped>
.tab section {
  display: unset;
}

.username {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-gap: 2rem;
}

fieldset {
  border: 0;
}

input {
  height: 4.5rem;
  background: white;
  border: 1px solid #D1D1D1;
  padding: 0 1rem;
  color: #333333;
  margin-bottom: 2.5rem;
  width: 100%;
}

input:focus {
  outline: 1px solid #333333;
  padding: 0 1rem;
}

.submit {
  background: #333333;
  height: 5rem;
  padding: 1rem 3rem;
  color: white;
  float: right;
  border: 0;
  font-weight: 500;
  font-size: 1.6rem;
  line-height: 2.3rem;
  text-transform: uppercase;
}
</style>
