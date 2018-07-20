<template>
  <section class="container">
    <div>
      <!--app-logo/-->
      <top-bar/>
      <slider/>
      <selling-types/>
            <div class="center">
            <div class="news" style="direction: rtl;color: darkgray;width: 30%;margin: 5px;">
                <br>
                <br>
                <br>
                <div style="text-align: center;">
                    <div>
                        <img src="../../pics/mail_icon_hover.png" alt="clothster" width="30%" height="auto"/>
                    </div>
                    در خبرنامه‌ی ما
                    <br>
                    <span style="color: #ffffff;">
                    <strong>
                        عضو شوید!
                    </strong>
                    </span>
                </div>
                <div style="text-align: center">
                    <div>
                        <input type="text" class="news_input" style="" placeholder="آدرس ایمیل خود را وارد کنید"/>
                        <input title="Search" value="&#9993;" type="button" class="news_button" style="width: 20%"/>
                    </div>
                </div>
                <br>
                <br>
                <div style="direction: ltr; text-align: center">
                    <button type="button" class="ozv">عضو شوید</button>
                </div>
                <br>
            </div>
            <div style="width: 70%; border:1px solid darkgray;margin: 5px;text-align: center;">
                <div class="centeroid_button">
                    <br>
                    <br>
                    <br>
                    <br>
                    <br>
                    <br>
                    <button type="button" class="tajrobe">تمام برندهای معتبر را با ما تجربه کنید</button>
                    <br>
                    <br>
                    <br>
                    <br>
                    <br>
                    <br>
                </div>
            </div>
            <br>
            <br>
        </div>
      <buttom-bar/>
    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'
import ButtomBar from '~/components/ButtomBar.vue'
import TopBar from '~/components/TopBar.vue'
import Slider from '~/components/Slider.vue'
import SellingTypes from '~/components/SellingTypes.vue'
export default {
  components: {
    AppLogo,
    ButtomBar,
    TopBar,
    Slider,
    SellingTypes
  }
}
</script>

<style scoped>
.news_input {
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
    border-radius: 25px 0 0 25px;
    margin-left: 5%;
}
.news_input:focus {
    outline: 0;
    background-color: #fff;
}
.news{
    background-color: #3232ff;
    box-shadow: 5px 5px 5px 5px #aaaaaa;

}
.center {
    display: flex;
    background-color: #f1f1f1;
}
.news_button {
    margin-top: 3.5%;
    background-color: rgba(255, 255, 255, 0.8);
    float: left;
    height: 32px;
    width: 20%;
    text-align: center;
    line-height: 32px;
    border: 0;
    color: #3232ff;
    font-size: 16px;
    text-rendering: auto;
    text-shadow: 0 1px 1px rgba(0, 0, 0, 0.2);
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    border-radius: 0 25px 25px 0;
}
.centeroid_button{
    background-image: url("../../pics/brands.png");
    position: relative;
    text-align: center;
    background-size: cover;
}
.tajrobe{
    font-size: 20px;
    border: 1px solid #6464ff;
    border-radius: 25px;
    width: 50%;
    color: #ffffff;
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    background-color: #3232ff;
}
.container {
  min-height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
.ozv {
    font-size: 10px;
    border: 1px solid #6464ff;
    border-radius: 25px;
    height: 32px;
    width: 30%;
    color: dodgerblue;
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    background-color: black;
}

.ozv:hover {
    -webkit-text-fill-color: rgba(255, 255, 255, 0.8);
    background-color: dodgerblue;
}
.links {
  padding-top: 15px;
}
</style>

