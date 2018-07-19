<template>
  <section class="container">
    <div>
      <!--app-logo/-->
      <top-bar/>
      <slider/>
      <selling-types/>
      <buttom-bar/>
    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'
import ButtomBar from '~/components/ButtomBar.vue'
import TopBar from '~/components/TopBar.vue'
import Slider from '~/components/Slider.vue'
import SellingTypes from '~/components/SellingTypes.vue'
export default {
  components: {
    AppLogo,
    ButtomBar,
    TopBar,
    Slider,
    SellingTypes
  }
}
</script>

<style scoped>
.container {
  min-height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

