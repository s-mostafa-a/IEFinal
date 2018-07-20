<template>
  <section class="container">
    <div>
    <top-bar/>
        <br>
    <user-info/>

        <br>

    <div>
    <b-btn @click="showCollapse1 = !showCollapse1"
           :class="showCollapse1 ? 'collapsed' : null"
           aria-controls="collapse4"
           :aria-expanded="showCollapse1 ? 'true' : 'false'" style="float: right;">
        آدرس‌ها
    </b-btn>
    <b-collapse class="mt-2" v-model="showCollapse1" id="collapse4">
        <br>
        <br>
        <br>
        <address-card/>
    </b-collapse>
    </div>
    <br>
    <br>
    <br>
    <b-btn @click="showCollapse = !showCollapse"
           :class="showCollapse ? 'collapsed' : null"
           aria-controls="collapse3"
           :aria-expanded="showCollapse ? 'true' : 'false'" style="float: right;">
        سفارشات
    </b-btn>
    <b-collapse class="mt-2" v-model="showCollapse" id="collapse3">
        <br>
        <br>
        <br>
        <buy-basket/>
    </b-collapse>

        <br>
        <br>
        <br>

      <buttom-bar/>
      </div>
  </section>
</template>
<script>
import ButtomBar from '~/components/ButtomBar.vue'
import TopBar from '~/components/TopBar.vue'
import UserInfo from '~/components/UserInfo.vue'
import AddressCard from '~/components/AddressCard.vue'
import BuyBasket from '~/components/BuyBasket.vue'





export default {
    data(){
        return{
            showCollapse1: true,
            showCollapse: false

        }
    },
  components: {
    ButtomBar,
    TopBar,
    UserInfo,
    AddressCard,
    BuyBasket

  }
}
</script>

<style scoped>
@font-face {
    font-family: "my_iran_sans";
    src: url("~/components/fonts/IRAN-sans.ttf");
}

* {
    font-family: "my_iran_sans";
}
</style>

