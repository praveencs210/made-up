<template>
  <section class="tab">
    <!--Profile Image-->
    <figure class="profie-container">
      <img class="profile-img" src="../../assets/img/profile.png">
      <hgroup>
        <h6 class="profile-name">Grishk</h6>
        <h2 class="profile-email">griiskaim@gmail.com</h2>
      </hgroup>
    </figure>
    <!--My Profile Section-->
    <MyProfile></MyProfile>
    <!--My Orders Section-->
    <MyOrders></MyOrders>
    <!--Shipping Address Section-->
    <Shipping></Shipping>
  </section>
</template>

<script>
import MyOrders from "@/components/profile/MyOrders";
import Shipping from "@/components/profile/Shipping";
import MyProfile from "@/components/profile/MyProfile";

export default {
  name: "Tabs",
  components: {MyProfile, Shipping, MyOrders}
}
</script>

<style>

.tab-item {
  /*margin: 2rem 0;*/
  display: flex;
}

.tab-heading {
  font-weight: 600;
  font-size: 2.4rem;
  line-height: 3.5rem;
  color: #777777;
  margin-top: 1rem;
  margin-bottom: 3rem;
}

.tab-title {
  font-weight: 600;
  font-size: 1.6rem;
  line-height: 2.3rem;
  color: #222222;
  margin: 0.5rem 0;
}

.tab__sub-title {
  color: #777777;
  padding-bottom: 0.5rem;
}

article {
  padding: 2rem;
  border: 1px solid #333333;
}

.tab-order {
  display: flex;
  flex-direction: column;
  width: 100%;
  margin-left: 2rem;
}

.tab-payment {
  width: 50%;
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

.tabs__order-img {
  height: 10rem;
  width: 10rem;
  margin-right: 2rem;
  object-fit: contain;
}

.tab__order-status {
  border-radius: 0.6rem 0.6rem 0 0;
  color: #FFFFFF;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 2.5rem;
  padding: 0 3rem;
}

.tab__order-pending {
  background: #333333;
}

.tab__order-delivered {
  background: #F3F3F3;
  color: #777777;
}

.tab-payment hgroup {
  text-align: right;
}

.tab__order-content {
  display: flex;
  margin: 2rem 0;
  border-bottom: 1px solid #DDDDDD;
}

.profie-container {
  display: flex;
  align-items: center;
  margin-bottom: 4rem;
}

.profile-img {
  width: 7.2rem;
  height: 7.2rem;
  object-fit: contain;
  border-radius: 50%;
  margin-right: 1rem;
}

.profile-name {
  font-weight: normal;
  font-size: 1.6rem;
  line-height: 2rem;
  color: #333333;
}

.profile-email {
  font-style: normal;
  font-weight: 500;
  font-size: 1.4rem;
  line-height: 2rem;
  color: #9B9B9B;
}
</style>
