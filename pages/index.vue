<template>
  <section class="container">
    <div>
      <top-bar/>
      <slider/>
      <br>
      <span style="float: right">
      محبوب ترین ها
      </span>
      <br>
      <product-slide/>
      <div>
<b-container fluid class="p-4 bg-dark">
  <b-row>
    <b-col style="height: 100px;text-align:center;margin:auto;color:white;font-size: 45px">
        بنر
    </b-col>
  </b-row>
</b-container>
      </div>
      <br>

      <br>

      <br>
      <br>
      <span style="float: right">
              

      جدید ترین ها
      </span>
      <br>
      <product-slide/>
      <div>
<b-container fluid class="p-4 bg-dark">
  <b-row>
    <b-col style="height: 100px;text-align:center;margin:auto;color:white;font-size: 45px">
        بنر
    </b-col>
  </b-row>
</b-container>
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
import Slider from '~/components/Slider.vue'




export default {
  components: {
    ButtomBar,
    TopBar,
    BrandBox,
    ColorBox,
    ProductCard,
    ProductType,
    SearchPageTop,
    ProductSlide,
    Slider

  },
  data(){
    return{
      image1: '~/assets/banner.png'}
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

