<template>
<div class="nav_bar_top">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <div style="width: 30%">
        <input type="text" class="search_box" placeholder="جست و جو"/>
        <input title="Search" value="&#128269;" type="button" class="search_button" style="width: 20%"/>
    </div>
    <div class="flex_grower" style="color: dimgray;">clothster</div>
    <div style="width: 30%">
    <div v-if="isLogin" id="cont" >
        <div style="text-align: center;">
        <b-button :size="size" variant="link">
        <i class="fa fa-list-alt"></i>
        <a href="" style="font-size: 10px;"> پیگیری سفارش 
        </a>
        </b-button>
        </div>
        <div>
        <b-button :size="size" variant="link">
            <i class="fa fa-shopping-basket"></i>
        <a href="" style="font-size: 10px;"> سبد خرید </a>
        </b-button>

        </div>
        <b-dropdown id="ddown1" variant="link" v-bind:text="name" size="sm">
            <b-dropdown-item>پروفایل</b-dropdown-item>
            <b-dropdown-item>سفارشات</b-dropdown-item>
            <b-dropdown-item>علایق</b-dropdown-item>
            <b-dropdown-divider></b-dropdown-divider>
            <b-dropdown-item>خروج</b-dropdown-item>
        </b-dropdown>
    </div>
    <div v-else>
        <button v-b-modal.vorood type="button" class="sign_in">ورود</button>
        <button v-b-modal.ozviat type="button" class="sign_up">عضویت</button>
            <login/>
            <register/>
    </div>
    </div>
</div>
</template>
<script>
import Login from '~/components/Login.vue'
import Register from '~/components/Register.vue'

export default {
    components:{
        Login,
        Register
    },
data() {
        //AJAX 
        // let info = fetch('my-api', {id: this.$route.params.id});
        return {
            isLogin: false,
            name: 'محمد رجبی',
        }
    },


}
</script>

<style scoped>
@font-face {
    font-family: "my_iran_sans";
    src: url("./fonts/IRAN-sans.ttf");
}
#ddown1{
    color: #212121;
    -webkit-text-fill-color: dimgray;        
}
#cont{
    display: flex;
}
* {
    font-family: "my_iran_sans";
}

.nav_bar_top {
    display: flex;
    background-color: #f1f1f1;
}

.nav_bar_top > div {
    background-color: #f1f1f1;
    margin: 10px;
    padding: 20px;
    font-size: 30px;
    text-align: center;
    width: 20%;
}
.flex_grower{
    flex-grow: 1;
}
.sign{
    font-size: 10px;
    border: 1px solid dimgray;
    border-radius: 25px;
    height: 32px;
    width: 30%;
    color: dimgray;
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    background-color: rgba(255, 255, 255, 0.8);
}
.search_box {
    direction: rtl;
    margin-top: 3.5%;
    height: 32px;
    width: 60%;
    line-height: 32px;
    padding: 0 16px;
    background-color: rgba(255, 255, 255, 0.8);
    color: #212121;
    border: 0;
    float: left;
    font-size: 12px;
    border-radius: 25px 0 0 25px;
}
.search_box:focus {
    outline: 0;
    background-color: #fff;
}
.search_button {
    margin-top: 3.5%;
    background-color: rgba(150, 150, 150, 0.8);
    float: left;
    height: 32px;
    width: 20%;
    text-align: center;
    line-height: 32px;
    border: 0;
    color: #fff;
    font-size: 16px;
    text-rendering: auto;
    text-shadow: 0 1px 1px rgba(0, 0, 0, 0.2);
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    border-radius: 0 25px 25px 0;
}
.search_button:hover {
    background-color: dodgerblue;
}
.sign:hover{
    -webkit-text-fill-color: rgba(255, 255, 255, 0.8);
    background-color: rgba(70, 70, 70, 0.8);
}
.sign_in{
    font-size: 10px;
    border: 1px solid dimgray;
    border-radius: 25px;
    height: 32px;
    width: 30%;
    color: white;
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    background-color: dimgray;
}
.sign_up{
    font-size: 10px;
    border: 1px solid dimgray;
    border-radius: 25px;
    height: 32px;
    width: 30%;
    color: dimgray;
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    background-color: rgba(255, 255, 255, 0.8);
}
.sign_in:hover{
    -webkit-text-fill-color: rgba(255, 255, 255, 0.8);
    background-color: dodgerblue;
    border: 1px solid dodgerblue;
}
.sign_up:hover{
    -webkit-text-fill-color: dodgerblue;
    color: dodgerblue;
    border: 1px solid dodgerblue;
}
</style>

