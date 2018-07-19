<template>
    <b-container fluid class="p-4 ">
      <b-row id="brow" style="direction: rtl;">
          <b-col> مشخصات محصول </b-col>
          <b-col> تعداد </b-col>
          <b-col> قیمت </b-col>
      </b-row>
      <b-row id="brow2" style="direction: rtl;">
          <b-col>
              <div style="display: flex;">
            <b-col>
                     <img :src="img" width="80px" height="80px">
              </b-col>
              <b-col style="font-size:8px">
                   {{brand}}<br>
                   {{prname}}<br>
                   {{color}}<br>
                   {{size}}<br>
                   {{code}}
               </b-col>
               </div>
          </b-col>
          <b-col style="display: flex;">
              {{no}}
          </b-col>
          <b-col> 
              {{price}}
          </b-col>
      </b-row>

      </b-container>
</template>
<script>
export default {
    data(){
        return{
            brand: 'brand',
            prname: 'product name',
            color: 'color',
            size: 'size',
            code: 'code',
            no: 'no',
            price: 'price'
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

#brow{
    background-color: gray;
    color: white;
}
#brow2{
    float: right;
    background-color: white;
    color: black;
}
</style>
