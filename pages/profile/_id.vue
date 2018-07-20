<template>
  <section class="container">
    <div>
    <top-bar/>
        <br>
    <user-info/>

        <br>

    <div>
    <b-btn @click="showCollapse = !showCollapse"
           :class="showCollapse ? 'collapsed' : null"
           aria-controls="collapse4"
           :aria-expanded="showCollapse ? 'true' : 'false'" style="float: right;">
        آدرس‌ها
    </b-btn>
    <b-collapse class="mt-2" v-model="showCollapse" id="collapse4">
        <br>
                <br>

        <br>

        <address-card/>
    </b-collapse>
    </div>


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




export default {
    data(){
        return{
            showCollapse: true
        }
    },
  components: {
    ButtomBar,
    TopBar,
    UserInfo,
    AddressCard,

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

