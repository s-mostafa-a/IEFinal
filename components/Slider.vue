<template>
<div id="Slider">
    <b-carousel 
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
                        :text="text1">
                          <b-img-lazy slot="img" class="d-block img-fluid w-100 my-5" :src="image1" center fluid-grow width="100" height="180" blank-color="#bbb" alt="img" />
      </b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide :caption="caption2"
                        :text="text2">
                          <b-img-lazy slot="img" class="d-block img-fluid w-100 my-5" :src="image2" center fluid-grow width="100" height="180" blank-color="#bbb" alt="img" />
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide :caption="caption3"
                        :text="text3">
                          <b-img-lazy slot="img" class="d-block img-fluid w-100 my-5" :src="image3" center fluid-grow width="100" height="180" blank-color="#bbb" alt="img" />
      </b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide :caption="caption4"
                        :text="text4">
                          <b-img-lazy slot="img" class="d-block img-fluid w-100 my-5" :src="image4" center fluid-grow width="100" height="180" blank-color="#bbb" alt="img" />
      </b-carousel-slide>
    </b-carousel>
    </div>
</template>
<script>
import axios from 'axios';

export default {/*
     created() {
    axios.get(`http://127.0.0.1:3000/homepage/`)
    .then(response => {
      // JSON responses are automatically parsed.
      console.log(response.data)
      //this.image1 = response.data.banners[0];
    })
    .catch(e => {
      this.errors.push(e)
    })
    },*/
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

@font-face {
    font-family: "my_iran_sans";
    src: url("./fonts/IRAN-sans.ttf");
}

* {
    font-family: "my_iran_sans";
}

    #Slider{
        text-align: center;
        width: 60%;
        margin-left: auto;
        margin-right: auto;
    }
</style>
