<template>
    <slider ref="slider" :pages="pages" :sliderinit="sliderinit">
    <!-- slot  -->
    </slider>
  </template>

  <script>
    import slider from 'vue-concise-slider'// import slider
    import ProductCard from '~/components/ProductCard.vue'
    module.exports = {
         components: {
              slider,
              ProductCard
         },
         data () {
            return {
              //Image list[arr]
              pages:[
                {
                  html: 'slide1',
                  style:{
                   'background': '#1bbc9b'
                  }
                },
                {
                 html: 'slide2',
                 style:{
                    background:'#4bbfc3'
                  }
                },
                {
                  html: 'slide3',
                  style:{
                    background:'#333'
                  },
                }
              ],
              // Sliding configuration[obj]
              sliderinit: {
                currentPage: 0,
                thresholdDistance: 100,
                thresholdTime: 300,
                loop:true,
                infinite:1,
                slidesToScroll:1
              }
            }
         }
    }
</script>