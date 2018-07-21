<template>
  <section class="container">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <top-bar/>
    <br><br><br>
  <div style="display: flex;dirction: rtl;padding:10px">
        <div style="width:50%;padding:20px">
      <span style="direction:rtl;">
                <br>
                              <div style="float:right;">

        برند {{brand}}<br>
        </div>
              <br>
                              <div style="float:right;">
        نام {{name}}<br>
                </div>
              <br>
                              <div style="float:right;">        قیمت {{price}}<br>
                        </div>
              <br>
                              <div style="float:right;">
        رنگ {{color}}<br>
                                </div>
              <br>
                              <div style="float:right;">
          <b-button size="lg" variant="danger">
افزودن به سبد خرید
            </b-button>
            <i class="fa fa-heart-o" style="font-size:48px;color:red"></i>
<br>
                                        </div>
                                        <br>
                                        <br>                                        <br>
                                        <br>
                              <div style="float:right;">
                              ویژگی ها:
                              <br>
                              <ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
    <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
                              </div>


      </span>
    
  </div>
    <div style="width:50%">
      <img src="https://i5.walmartimages.com/asr/9ad142d8-09c5-43c9-a618-646f75701d38_1.aca00e67749f0075fa12c4ee2f488510.jpeg?odnHeight=450&odnWidth=450&odnBg=FFFFFF"/>
  </div>

  </div>
  <div>
      <b-tabs>
  <b-tab title="first" active>
    <br>I'm the first fading tab
  </b-tab>
  <b-tab title="second" >
    <br>I'm the second tab content
  </b-tab>
  <b-tab title="disabled" disabled>
    <br>Disabled tab!
  </b-tab>
</b-tabs>
  </div>






    <div>
      <br>
      <br>
      <br>
      <br>
      <span style="float: right">
محصولات  مرتبط
      </span>
      <br>
      <product-slide/>
      <div>
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
      image1: '~/assets/banner.png',
      price: 1000,
      color: 'زرد',
      brand: 'برند',
      name: 'کفش'
      }
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

