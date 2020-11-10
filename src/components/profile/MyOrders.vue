<template>
  <section class="tab-item" id="section1">
    <input type="radio" name="sections" id="option1">
    <label for="option1">
      <h1 class="tab-title">My Orders</h1>
      <p class="tab__sub-title">Notifications, password</p>
    </label>
    <article class="tab-content">
      <h1 class="tab-heading">My Orders</h1>
      <!--Orders 1-->
      <section class="tab__order-content">
        <figure>
          <img class="tabs__order-img" src="../../assets/img/orders.png">
        </figure>
        <section class="tab-order">
          <hgroup class="tab__order-details">
            <p class="tab__sub-title">Order #12345678</p>
            <p class="tab__sub-title">Credit Card Payment</p>
          </hgroup>

          <hgroup class="tab__order-details">
            <h1 class="tab-title">Madeup White Cotton Blend <br/> Checkered Slim Fit Shirt</h1>
            <h1 class="tab-title">Rs 1,899</h1>
          </hgroup>

          <hgroup class="tab__order-details">
            <p class="tab__sub-title">Express Delivery by Sat, Aug 30</p>
            <i class="fa fa-chevron-down" aria-hidden="true"></i>
          </hgroup>

          <hgroup class="tab__order-details">
            <p></p>
            <p class="tab__order-status tab__order-pending">Pending</p>
          </hgroup>
        </section>
      </section>
      <!--Orders 2-->
      <section class="tab__order-content">
        <figure>
          <img class="tabs__order-img" src="../../assets/img/orders.png">
        </figure>
        <section class="tab-order">
          <hgroup class="tab__order-details">
            <p class="tab__sub-title">Order #12345678</p>
            <p class="tab__sub-title">Credit Card Payment</p>
          </hgroup>

          <hgroup class="tab__order-details">
            <h1 class="tab-title">Madeup White Cotton Blend <br/> Checkered Slim Fit Shirt</h1>
            <h1 class="tab-title">Rs 1,899</h1>
          </hgroup>

          <hgroup class="tab__order-details">
            <p class="tab__sub-title">Express Delivery by Sat, Aug 30</p>
            <i class="fa fa-chevron-down" aria-hidden="true"></i>
          </hgroup>

          <hgroup class="tab__order-details">
            <p></p>
            <p class="tab__order-status tab__order-pending">Pending</p>
          </hgroup>
        </section>
      </section>
      <!--Orders 3-->
      <section class="tab__order-content">
        <figure>
          <img class="tabs__order-img" src="../../assets/img/orders.png">
        </figure>
        <section class="tab-order">
          <hgroup class="tab__order-details">
            <p class="tab__sub-title">Order #12345678</p>
            <p class="tab__sub-title">Credit Card Payment</p>
          </hgroup>

          <hgroup class="tab__order-details">
            <h1 class="tab-title">Madeup White Cotton Blend <br/> Checkered Slim Fit Shirt</h1>
            <h1 class="tab-title">Rs 1,899</h1>
          </hgroup>

          <hgroup class="tab__order-details">
            <p class="tab__sub-title">Express Delivery by Sat, Aug 30</p>
            <i class="fa fa-chevron-down" aria-hidden="true"></i>
          </hgroup>

          <hgroup class="tab__order-details">
            <p></p>
            <p class="tab__order-status tab__order-delivered">Delivered</p>
          </hgroup>
        </section>
      </section>
      <!--Orders 4-->
      <section class="tab__order-content">
        <figure>
          <img class="tabs__order-img" src="../../assets/img/orders.png">
        </figure>
        <section class="tab-order">
          <hgroup class="tab__order-details">
            <p class="tab__sub-title">Order #12345678</p>
            <p class="tab__sub-title">Credit Card Payment</p>
          </hgroup>

          <hgroup class="tab__order-details">
            <h1 class="tab-title">Madeup White Cotton Blend <br/> Checkered Slim Fit Shirt</h1>
            <h1 class="tab-title">Rs 1,899</h1>
          </hgroup>

          <hgroup class="tab__order-details">
            <p class="tab__sub-title">Express Delivery by Sat, Aug 30</p>
            <i class="fa fa-chevron-down" aria-hidden="true"></i>
          </hgroup>

          <hgroup class="tab__order-details">
            <p></p>
            <p class="tab__order-status tab__order-delivered">Delivered</p>
          </hgroup>
        </section>
      </section>
    </article>
  </section>
</template>

<script>
export default {
  name: "MyOrders"
}
</script>

<style scoped>
.tab__order-details {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
