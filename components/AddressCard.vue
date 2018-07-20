<template>
<div class="tg-wrap">
    <div>
    <img src='../pics/addr.png' height="100px"/>
    </div>
    <br>
    <br>
    <div style="margin: auto;">
        :هزینه ارسال
        <div style="color: #18bbb9;">
            <span style="font-size: 20px">{{send_price}}&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br><span style="font-size:15px">تومان</span></span> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        </div>
        
    </div>
    <div>
    <table class="tg">
  <tr>
    <td class="tg-llds"></td>
    <td class="tg-pig6"></td>
    <td class="tg-pig6"></td>
    <td class="tg-pig6"></td>
    <td class="tg-u6j1" rowspan="2"></td>
  </tr>
  <tr>
    <td class="tg-4fnb"></td>
    <td class="tg-u6j1"></td>
    <td class="tg-u6j1" colspan="2"></td>
  </tr>
</table>
    </div>
</div>
</template>

<script>
export default {
    props: ['selected'],
    data(){
        return{
            name: 'نام',
            send_price: 30000,
        items: [
        { 1:"تحویل گیرنده: " ,2:'Dickerson', 3:'Macdonald' },
      ],
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
.tg-wrap{width: 100%;margin: auto;text-align: center;}
.tg  {border-collapse:collapse;border-spacing:0;border-color:#ccc;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#fff;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#f0f0f0;}
.tg .tg-pig6{background-color:#ffffff;border-color:#38fff8;vertical-align:top}
.tg .tg-llds{background-color:#efefef;border-color:#38fff8;text-align:right;vertical-align:top}
.tg .tg-u6j1{border-color:#38fff8;vertical-align:top}
.tg .tg-4fnb{background-color:#efefef;border-color:#38fff8;vertical-align:top}
</style>