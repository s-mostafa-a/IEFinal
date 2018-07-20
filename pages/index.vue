<template>
  <section class="container">
    <div>
      <top-bar/>
      <div style="display:flex;direction:rtl;">
        <div style="width: 20%">
          <product-type/>
      <color-box/>
      </div>


      </div>






      <brand-box/>
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

