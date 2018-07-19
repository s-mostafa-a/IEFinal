<template>
<div>
    <login-part/>
    <div class="nav_bar_down">
    <div class="flex_grower" style="width: 20%;">
    </div>
    <div style="font-size: 10px;">
        <input title="برندها" value="برندها" type="button" class="nav_icon"/>
    </div>
    <div style="font-size: 10px;">
        <input title="تخفیف" value="تخفیف" type="button" class="nav_icon"/>
    </div>
    <div style="font-size: 10px;">
        <input title="ورزشی" value="ورزشی" type="button" class="nav_icon"/>
    </div>
    <div style="font-size: 10px;">
        <input title="بچگانه" value="بچگانه" type="button" class="nav_icon"/>
    </div>
    <div style="font-size: 10px;">
        <input title="زنانه" value="زنانه" type="button" class="nav_icon"/>
    </div>
    <div style="font-size: 10px;">
        <input title="مردانه" value="مردانه" type="button" class="nav_icon"/>
    </div>
    <div class="flex_grower" style="width: 20%">
    </div>
</div>
</div>
</template>
<script>
import LoginPart from './LoginPart.vue';
export default {
  components: {
      LoginPart,
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

.nav_bar_down {
    margin-top: 1px;
    padding: 0px;
    display: flex;
    background-color: #f1f1f1;

}

.nav_bar_down > div {
    background-color: #f1f1f1;
    text-align: center;
    height: 100%;
    width: 7%;
}
.flex_grower{
    flex-grow: 1;
}

.nav_icon{
    background-color: #f1f1f1;
    height: 100%;
    width: 100%;
    text-align: center;
    border: 0;
    color: dimgray;
    text-rendering: auto;
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
}
.nav_icon:hover {
    background-color: rgba(70, 70, 70, 0.8);
    color: white;
}


</style>
