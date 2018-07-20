<template>
  <section class="container">
    <div>
    <login-part/>
      <address-card/>
      <buttom-bar/>
      </div>
  </section>
</template>

<script>
import ButtomBar from '~/components/ButtomBar.vue'
import TopBar from '~/components/TopBar.vue'
import LoginPart from '~/components/LoginPart.vue'
import UserInfo from '~/components/UserInfo.vue'
import AddressCard from '~/components/AddressCard.vue'


export default {
  components: {
    ButtomBar,
    TopBar,
    LoginPart,
    UserInfo,
    AddressCard

  }
}
</script>

<style scoped>

</style>

