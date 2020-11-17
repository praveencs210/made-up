<template>
  <section class="tab-item" id="section1">
    <input type="radio" name="sections" id="option1">
    <label for="option1">
      <h1 class="tab-title">My Orders</h1>
      <p class="tab__sub-title">Notifications, password</p>
    </label>
    <article class="tab-content">
      <section class="tab_container">
        <!--Pending Orders-->
        <input id="tab1" type="radio" name="tabs" checked>
        <label for="tab1">Pending Orders</label>

        <!--Past Orders-->
        <input id="tab2" type="radio" name="tabs">
        <label for="tab2">Past Orders</label>

        <!--Pending Orders Content-->
        <section id="content1" class="orders-tab-content">
          <!--Orders 1-->
          <details v-for="order in orders" v-bind:key="order">
            <summary v-if="order.deliveryStatus==false">
              <section class="tab__order-content">
                <figure>
                  <img class="tabs__order-img" :src="order.productImg">
                </figure>
                <section class="tab-order">
                  <hgroup class="tab__order-details">
                    <p class="tab__sub-title">{{ order.orderID }}</p>
                    <p class="tab__sub-title">{{ order.payment }}</p>
                  </hgroup>

                  <hgroup class="tab__order-details">
                    <h1 class="tab-title">{{ order.productName }}</h1>
                    <h1 class="tab-title">{{ order.price }}</h1>
                  </hgroup>

                  <hgroup class="tab__order-details">
                    <p class="tab__sub-title">{{ order.deliveryDate }}</p>
                    <i class="fa fa-chevron-down" aria-hidden="true"></i>
                  </hgroup>
                </section>
              </section>
            </summary>
            <section v-if="order.deliveryStatus==false" class="order-track">
              <hgroup class="order-track-step">
                <p class="order-track-status">
                  <span class="order-track-status-dot"></span>
                  <span class="order-track-status-line"></span>
                </p>
                <div class="order-track-text">
                  <p class="order-track-text-stat">Order Recieved</p>
                  <p class="order-track-text-sub">{{ order.received }}</p>
                </div>
              </hgroup>
              <hgroup class="order-track-step">
                <p class="order-track-status">
                  <span class="order-track-status-dot"></span>
                  <span class="order-track-status-line"></span>
                </p>
                <div class="order-track-text">
                  <p class="order-track-text-stat"> Order Dispactched </p>
                  <p class="order-track-text-sub">{{ order.dispatched }}</p>
                </div>
              </hgroup>
              <hgroup class="order-track-step">
                <p class="order-track-status">
                  <span class="order-track-status-dot"></span>
                  <span class="order-track-status-line"></span>
                </p>
                <div class="order-track-text">
                  <p class="order-track-text-stat"> Order Reached </p>
                  <p class="order-track-text-sub">{{ order.reached }}</p>
                </div>
              </hgroup>
              <hgroup class="order-track-step">
                <p class="order-track-status">
                  <span class="order-track-status-dot"></span>
                  <span class="order-track-status-line"></span>
                </p>
                <div class="order-track-text">
                  <p class="order-track-text-stat"> {{ order.delivered }} </p>
                </div>
              </hgroup>
            </section>
          </details>
        </section>

        <!--Past Orders Content-->
        <section id="content2" class="orders-tab-content">
          <!--Orders 2-->
          <details v-for="order in orders" v-bind:key="order">
            <summary v-if="order.deliveryStatus==true">
              <section class="tab__order-content">
                <figure>
                  <img class="tabs__order-img" :src="order.productImg">
                </figure>
                <section class="tab-order">
                  <hgroup class="tab__order-details">
                    <p class="tab__sub-title">{{ order.orderID }}</p>
                    <p class="tab__sub-title">{{ order.payment }}</p>
                  </hgroup>

                  <hgroup class="tab__order-details">
                    <h1 class="tab-title">{{ order.productName }}</h1>
                    <h1 class="tab-title">{{ order.price }}</h1>
                  </hgroup>

                  <hgroup class="tab__order-details">
                    <p class="tab__sub-title">{{ order.deliveryDate }}</p>
                    <i class="fa fa-chevron-down" aria-hidden="true"></i>
                  </hgroup>
                </section>
              </section>
            </summary>
            <section v-if="order.deliveryStatus==true" class="order-track">
              <hgroup class="order-track-step">
                <p class="order-track-status">
                  <span class="order-track-status-dot"></span>
                  <span class="order-track-status-line"></span>
                </p>
                <div class="order-track-text">
                  <p class="order-track-text-stat">Order Recieved</p>
                  <p class="order-track-text-sub">{{ order.received }}</p>
                </div>
              </hgroup>
              <hgroup class="order-track-step">
                <p class="order-track-status">
                  <span class="order-track-status-dot"></span>
                  <span class="order-track-status-line"></span>
                </p>
                <div class="order-track-text">
                  <p class="order-track-text-stat"> Order Dispactched </p>
                  <p class="order-track-text-sub">{{ order.dispatched }}</p>
                </div>
              </hgroup>
              <hgroup class="order-track-step">
                <p class="order-track-status">
                  <span class="order-track-status-dot"></span>
                  <span class="order-track-status-line"></span>
                </p>
                <div class="order-track-text">
                  <p class="order-track-text-stat"> Order Reached </p>
                  <p class="order-track-text-sub">{{ order.reached }}</p>
                </div>
              </hgroup>
              <hgroup class="order-track-step">
                <p class="order-track-status">
                  <span class="order-track-status-dot"></span>
                  <span class="order-track-status-line"></span>
                </p>
                <div class="order-track-text">
                  <p class="order-track-text-stat"> {{ order.delivered }} </p>
                </div>
              </hgroup>
            </section>
          </details>
        </section>
      </section>
    </article>
  </section>
</template>

<script>
import axios from 'axios';

export default {
  name: "MyOrders",
  data() {
    return {
      orders: []
    }
  },
  methods: {
    fetchPosts() {
      axios.get("http://localhost:3000/orders").then(response => (this.orders = response.data));
      console.log("Hello")
    }
  },
  mounted() {
    this.fetchPosts();
  }
}
</script>

<style scoped>
.tab__order-details {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.tab_container {
  width: 100%;
  position: relative;
}

.tab_container label {
  font-weight: 500 !important;
  font-size: 2.4rem !important;
  line-height: 3.5rem;
  color: #777777;
  margin: 0;
  text-align: center !important;
  width: 50%;
}

.tab_container label:before {
  content: ''
}

input, .orders-tab-content {
  clear: both;
  padding-top: 10px;
  display: none;
}

.orders-tab-content {
  border-top: 1px solid #333333 !important;
  border-bottom: none !important;
}

.tab_container label {
  font-weight: 500;
  font-size: 18px;
  display: block;
  float: left;
  color: #757575;
  cursor: pointer;
  text-decoration: none;
  text-align: center;
}

#tab1:checked ~ #content1,
#tab2:checked ~ #content2 {
  display: block;
  padding: 20px;
  background: #fff;
  color: #999;
  border-bottom: 1px solid #DDDDDD;
}

.tab_container [id^="tab"]:checked + label {
  background: #fff;
  color: #333333;
  border-bottom: 1px solid #000000;
}

summary {
  cursor: pointer;
}

summary::-webkit-details-marker {
  display: none
}

summary:focus {
  outline: none;
}

details {
  border-bottom: 1px solid #DDDDDD;
}

.order-track {
  padding: 2rem 0 3rem 3rem;
  display: flex;
  flex-direction: column;
}

.order-track-step {
  display: flex;
  height: 7rem;
}

.order-track-step:last-child {
  overflow: hidden;
  height: 4rem;
}

.order-track-step:last-child .order-track-status span:last-of-type {
  display: none;
}

.order-track-status {
  margin-right: 1.5rem;
  position: relative;
}

.order-track-status-dot {
  display: block;
  width: 2.2rem;
  height: 2.2rem;
  border-radius: 50%;
  background: white;
  border: 1px solid #DDDDDD;
}

.order-track-status-line {
  display: block;
  margin: 0 auto;
  width: 2px;
  height: 7rem;
  background: #DDDDDD;
}

.order-track-text-stat {
  font-style: normal;
  font-weight: 500;
  font-size: 1.6rem;
  line-height: 2.3rem;
  color: #333333;
}

.order-track-text-sub {
  font-style: normal;
  font-weight: 500;
  font-size: 1.3rem;
  line-height: 2.3rem;
  color: #777777;
}

details:empty{
  display: none;
}

</style>
