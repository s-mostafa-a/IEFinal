<template>
  <section class="container">
    <div>
      <top-bar/>
      <br>
      <br>
      <div style="display:flex;direction:rtl;">
        <div style="width: 20%">
          <product-type/>
                <br>

                <brand-box/>
                      <br>

      <color-box/>
      </div>
      <div style="padding: 20px">
        <search-page-top/>
        <hr>

        <div style="display: flex;">
          <div v-for="i in 4" :key="i" style=" margin: 10px">
        <product-card/>
        </div>
        </div>
                <div style="display: flex;">
          <div v-for="i in 4" :key="i" style=" margin: 10px">
        <product-card/>
        </div>
        </div>
                <div style="display: flex;">
          <div v-for="i in 4" :key="i" style=" margin: 10px">
        <product-card/>
        </div>
        </div>
                <div style="display: flex;">
          <div v-for="i in 4" :key="i" style=" margin: 10px">
        <product-card/>
        </div>
        </div>
      </div>

      </div>






      <buttom-bar/>
      </div>
  </section>
</template>

<script>
import ButtomBar from '~/components/ButtomBar.vue'
import TopBar from '~/components/TopBar.vue'
import BrandBox from '~/components/BrandBox.vue'
import ColorBox from '~/components/ColorBox.vue'
import ProductCard from '~/components/ProductCard.vue'
import ProductType from '~/components/ProductType.vue'
import SearchPageTop from '~/components/SearchPageTop.vue'
import ProductSlide from '~/components/ProductSlide.vue'




export default {
  components: {
    ButtomBar,
    TopBar,
    BrandBox,
    ColorBox,
    ProductCard,
    ProductType,
    SearchPageTop,
    ProductSlide

  }
}
</script>

<style scoped>

</style>

