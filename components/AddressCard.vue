<template>
<div class="tg-wrap">
    <div>
    <img src='../pics/addr.png' height="100px"/>
    </div>
    <br>
    <br>
    <div style="margin: auto; text-align:center">
        :هزینه ارسال
        <div style="color: #18bbb9;">
            <span style="font-size: 20px">{{send_price}}&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br><span style="font-size:15px">تومان</span></span> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        </div>
        
    </div>
    <div style="direction: rtl;width: 100%;margin: auto;text-align: center;">
    <form action="/Cart/Shipping" method="post" id="changeAddressForm" novalidate="novalidate">
            <div class="address-list">

                    <div class="table-container checked-table" id="recipient_318463">
                        <table class="table" style="background-color: white;     border: 1px solid darkturquoise;">
                            <colgroup>
                                <col class="radio-box-col">
                            </colgroup>

                            <tbody>

                                <tr style="border: 1px solid darkturquoise;">
                                    <td rowspan="2" class="table-radio table-radio-checked" style="border: 1px solid darkturquoise;">
                                        <label class="custom-radio">
                                            <input type="radio" disabled name="shipping_address" value="" :checked="checked1">
                                            <span></span>
                                        </label>
                                    </td>
                                    <td colspan="1" class="shipping__name" width="27%" style="border: 1px solid darkturquoise;">
                                        <span class="title">تحویل گیرنده:</span>
                                        <span class="value">{{name}}</span>
                                    </td>
                                    <td colspan="1" style="border: 1px solid darkturquoise;">
                                        <span class="title">شماره تماس ثابت:</span>
                                        <span class="value">{{home_no}}</span>
                                    </td>
                                    <td colspan="1" width="25%" style="border: 1px solid darkturquoise;">
                                        <span class="title">شماره تماس اضطراری:</span>
                                        <span class="value">{{mobile}}</span>
                                    </td>
                                    <td rowspan="3" class="action-cell" style="border: 1px solid darkturquoise;">
                                        <table class="action-table">
                                            <tbody ><tr>
                                                <td class="edit" style="border: 1px solid darkturquoise;">
                                                    <a href="">
                                                             <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
                                                            <i class="fa fa-pencil"></i>
                                                    </a>
                                                </td>
                                            </tr>
                                            <tr>
                                                <td class="delete" style="border: 1px solid darkturquoise;">
                                                    <a href="">
                                                        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
                                                        <i class="fa fa-close"></i>

                                                    </a>
                                                </td>
                                            </tr>
                                        </tbody></table>
                                    </td>
                                </tr>

                                <tr style="border: 1px solid darkturquoise;">
                                    <td class="shipping__address" colspan="2" style="border: 1px solid darkturquoise;">
                                        <span class="title">آدرس:</span>
                                        <span class="value">{{address}}</span>
                                    </td>
                                    <td colspan="1" width="25%" style="border: 1px solid darkturquoise;">
                                        <span class="title">کد پستی:</span>
                                        <span class="value">{{postal_code}}</span>
                                    </td>
                                </tr>

                            </tbody>

                        </table>
                    </div>
            </div>

        </form>
    </div>

    <div v-for="i in number" style="direction: rtl;width: 100%;margin: auto;text-align: center;" :key="i" >
    <form action="/Cart/Shipping" method="post" :id="i" novalidate="novalidate">
            <div class="address-list">
                    <div class="table-container" id="recipient_318463">
                        <table class="table">

                            <colgroup>
                                <col class="radio-box-col">
                            </colgroup>

                            <tbody>

                                <tr>
                                    <td rowspan="2" class="table-radio table-radio-checked">
                                        <label class="custom-radio">
                                            <input disabled type="radio" name="shipping_address" value="" :checked="checked2">
                                            <span></span>
                                        </label>
                                    </td>
                                    <td colspan="1" class="shipping__name" width="27%">
                                        <span class="title">تحویل گیرنده:</span>
                                        <span class="value">{{name}}</span>
                                    </td>
                                    <td colspan="1">
                                        <span class="title">شماره تماس ثابت:</span>
                                        <span class="value">{{home_no}}</span>
                                    </td>
                                    <td colspan="1" width="25%">
                                        <span class="title">شماره تماس اضطراری:</span>
                                        <span class="value">{{mobile}}</span>
                                    </td>
                                    <td rowspan="3" class="action-cell">
                                        <table class="action-table">
                                            <tbody><tr>
                                                <td class="edit">
                                                    <a href="">
                                                             <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
                                                            <i class="fa fa-pencil"></i>
                                                    </a>
                                                </td>
                                            </tr>
                                            <tr>
                                                <td class="delete">
                                                    <a href="">
                                                        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
                                                        <i class="fa fa-close"></i>

                                                    </a>
                                                </td>
                                            </tr>
                                        </tbody></table>
                                    </td>
                                </tr>

                                <tr>
                                    <td class="shipping__address" colspan="2">
                                        <span class="title">آدرس:</span>
                                        <span class="value">{{address}}</span>
                                    </td>
                                    <td colspan="1" width="25%">
                                        <span class="title">کد پستی:</span>
                                        <span class="value">{{postal_code}}</span>
                                    </td>
                                </tr>

                            </tbody>

                        </table>
                    </div>
            </div>

        </form>
    </div>
    <button type="button" class="tajrobe"> اضافه کردن آدرس جدید </button>
    <br>
    <br>
    <div style="float: right;">
        <span style="color: dimgray;">زمان دریافت سفارش</span>
        <div dir="rtl">
  <b-dropdown id="ddown-header" :text="day" class="m-2">
    <b-dropdown-header>{{day}}</b-dropdown-header>
        <b-dropdown-item-button>{{day1}}</b-dropdown-item-button>
    <b-dropdown-item-button>{{day2}}</b-dropdown-item-button>
    <b-dropdown-item-button>{{day3}}</b-dropdown-item-button>
  </b-dropdown>
  <br>
</div>
    </div>
    <br>
    <br>
    <br>
    <br>
          <button type="button" class="tajrobe" style="height: 40px"> ثبت و مرحله بعد </button>
    <br>
    
</div>
</template>

<script>
export default {
    data(){
        return{
            checked1: true,
            checked2: false,
            postal_code: '10',
            address: 'address',
            home_no:'phone',
            mobile: 'mobile',
            name:'name',
            number:2,
            send_price: 30000,
            day: 'شنبه',
            day1:'یکشنبه',
            day2:'دوشنبه',
            day3:'سه شنبه'
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
    width: 20%;
    color: #ffffff;
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    background-color: #3232ff;
}
.table  {    border: 1px solid black;
background-color:lightgray;}
.table td{    border: 1px solid black;
font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;color:#333;}
.table th{    border: 1px solid black;
font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
</style>