<template>
  <section class="container">
    <div>
    <login-part/>
        <div>
    <img src='../../pics/addr.png' height="100px"/>
    </div>
    <br>
    <br>
    <div style="margin: auto; text-align:center">
        :هزینه ارسال
        <div style="color: #18bbb9;">
            <span style="font-size: 20px">{{send_price}}&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br><span style="font-size:15px">تومان</span></span> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        </div>
        
    </div>
      <address-card/>
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
      <buttom-bar/>
      </div>
  </section>
</template>

<script>
import ButtomBar from '~/components/ButtomBar.vue'
import TopBar from '~/components/TopBar.vue'
import LoginPart from '~/components/LoginPart.vue'
import UserInfo from '~/components/UserInfo.vue'
import AddressCard from '~/components/AddressCard.vue'


export default {
  data(){
    return{
      send_price: 3000
    }
  },
  components: {
    ButtomBar,
    TopBar,
    LoginPart,
    UserInfo,
    AddressCard

  }
}
</script>

<style scoped>
@font-face {
    font-family: "my_iran_sans";
    src: url("~/components/fonts/IRAN-sans.ttf");
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
</style>

