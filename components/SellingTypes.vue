<template>
<b-container fluid class="p-4 ">
  <b-row>
          <b-col>
          </b-col>
    <b-col class="col">
      <b-img thumbnail fluid :src="image1" alt="Thumbnail" /> 
            <div style="background-color: gray;">

      مردانه
            </div>
    </b-col>
    <b-col class="col">
      <b-img thumbnail fluid :src="image2" alt="Thumbnail" />
      <div style="background-color: gray;">
      زنانه
      </div>
    </b-col>
    <b-col class="col">
      <b-img thumbnail fluid :src="image3" alt="Thumbnail" />
            <div style="background-color: gray;">
      بچگانه
            </div>
    </b-col>
              <b-col>
          </b-col>
  </b-row>
</b-container>
</template>

<script>
export default {
    data(){
        return{
            image1:'https://picsum.photos/1024/480/?image=52',
            image2:'https://picsum.photos/1024/480/?image=52',
            image3:'https://picsum.photos/1024/480/?image=52'
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

.col{
    background-color:white;
    color: white;
}
</style>

