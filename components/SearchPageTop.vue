<template>
    <div style="display: flex;margin:auto;">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
            <b-button size="sm" variant="secondary">      
            <i class="fa fa-caret-square-o-left" @click="dec" style="font-size:36px"></i>

            </b-button> <div style="text-align: center;margin:auto;">
            صفحه‌ی {{page_no}} از {{page_max}}
            </div>
            <b-button size="sm" v-on:click="inc" variant="secondary">
                <i class="fa fa-caret-square-o-right" style="font-size:36px"></i>
            </b-button> 

            <br>
    </div>
</template>
<script>
export default {
    data(){
        return{
            page_no: 1,
            page_max: 10
        }
    },
    methods:{
        inc: function(){
            page_no += 2;
            page_no %= 10;
            alert(6)
        },
        dec: function(){
            page_no -= 1;
            page_no %= 10;
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
