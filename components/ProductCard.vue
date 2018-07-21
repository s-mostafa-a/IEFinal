<template>
    <div style="padding: 10px">
        <b-card :title="mahsool"
          img-src="https://i5.walmartimages.com/asr/9ad142d8-09c5-43c9-a618-646f75701d38_1.aca00e67749f0075fa12c4ee2f488510.jpeg?odnHeight=450&odnWidth=450&odnBg=FFFFFF"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 200px;"
          class="mb-2"
          >
            <div class="card-text" style="direction: rtl; float: right;">
                <div style="font-size: 25px">بوت</div>
                <div>{{price}} تومان</div>
            </div>
        </b-card>
    </div>
</template>
<script>
export default {
    data(){
        return{
            price: 1000,
            mahsool: 'Nader',
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
</style>
