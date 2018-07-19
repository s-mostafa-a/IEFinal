<template>
    <b-carousel id="Slider"
                style="text-shadow: 1px 1px 2px #333;"
                controls
                indicators
                background="#ababab"
                :interval="4000"
                img-width="100"
                img-height="180"
                v-model="slide"
                @sliding-start="onSlideStart"
                @sliding-end="onSlideEnd"
    >

      <!-- Text slides with image -->
      <b-carousel-slide :caption="caption1"
                        :text="text1"
                        :img-src="image1"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide :caption="caption2"
                        :text="text2"
                        :img-src="image2">
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide :caption="caption3"
                        :text="text3"
                        :img-src="image3">
      </b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide :caption="caption4"
                        :text="text4"
                        :img-src="image4">
      </b-carousel-slide>
    </b-carousel>
</template>
<script>
export default {
    data () {
    return {
        text1: 'text1',
        text2: 'text2',
        text3: 'text3',
        text4: 'text4',
        caption1: 'caption1',
        caption2: 'caption2',
        caption3: 'caption3',
        caption4: 'caption4',
        image1: 'https://picsum.photos/1024/480/?image=52',
        image2: 'https://picsum.photos/1024/480/?image=54',
        image3: 'https://picsum.photos/1024/480/?image=56',
        image4: 'https://picsum.photos/1024/480/?image=58',

        slide: 0,
        sliding: null
    }
  },
  methods: {
    onSlideStart (slide) {
      this.sliding = true
    },
    onSlideEnd (slide) {
      this.sliding = false
    }
  }
}
</script>
<style scoped>

</style>
