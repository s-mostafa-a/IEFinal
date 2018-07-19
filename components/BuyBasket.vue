<template>
<div>
    <b-container fluid class="p-4 ">
      <b-row id="brow" style="direction: rtl;">
          <b-col> مشخصات محصول </b-col>
          <b-col> تعداد </b-col>
          <b-col> قیمت </b-col>
      </b-row>
      <b-row id="brow2" style="direction: rtl;">
          <b-col style="display: flex;">
              <b-col>
                     <img :src="img" width="80px" height="80px">
              </b-col>
              <b-col style="font-size:8px; float: right;">
                   {{brand}}<br>
                   {{prname}}<br>
                   {{color}}<br>
                   {{size}}<br>
                   {{code}}
               </b-col>

          </b-col>
          <b-col style="margin: auto;">
              {{no}}
          </b-col>
          <b-col style="margin: auto;"> 
              {{price}}
          </b-col>
      </b-row>
      </b-container>
<button type="button" class="tajrobe">ثبت و مرحله بعد</button>

</div>
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

.tajrobe{
    float: left;
    font-size: 100%;
    border: 1px solid #6464ff;
    border-radius: 25px;
    width: 15%;
    color: #ffffff;
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    background-color: #3232ff;
}
#brow{
    background-color: gray;
    color: white;
}
#brow2{
    background-color: white;
    color: black;
}
</style>
