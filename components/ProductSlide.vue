<template>
      <b-card>
  <div style="display: flex;margin: auto; padding: 10px">

      <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
      <div style="text-align: center;margin: auto">
                  <a href="">
<i class="fa fa-caret-square-o-left" style="font-size:48px;color:gray"></i>
                  </a>
      </div>
      <product-card/>
            <product-card/>
      <product-card/>



      <product-card/>
      <product-card/>


      <product-card/>

      <product-card/>

    <div style="text-align: center;margin: auto">
        <a href="">
<i class="fa fa-caret-square-o-right" style="font-size:48px;color:gray"></i>
        </a>
    </div>
  </div>
      </b-card>

</template>
 
<script>
import ProductCard from '~/components/ProductCard.vue'
export default {
    components:{
        ProductCard
    },
  data () {
    return {
        gt: '>',
        lt: '<'
  }
  }
}
</script>