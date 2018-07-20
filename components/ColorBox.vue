<template>
    <div>
<div dir="rtl" style="display: flex">
<b-btn  variant="outline-success" v-b-toggle.myCollapse >
  <span class="when-opened">رنگ -</span>
  <span class="when-closed">رنگ +</span>
</b-btn>
</div>
<b-collapse id="myCollapse">
  <!-- content here -->
<b-card>
<div class="product-color select-option clearfix">
                                <span>
                                    <div style="display: flex; margin: auto">
                                    <div id="nearby-6-wrapper" style="margin:2px;width:15%;background-color: #000000" title="مشکی">
                                    <br></div>

                                    <div id="nearby-37-wrapper" style="margin:2px;width:15%;background-color: #0000ff" title="آبی">
                                    <br></div>

                                    <div id="nearby-39-wrapper" style="margin:2px;width:15%;background-color: #000080" title="سرمه ای">
                                    <br></div>

                                    <div id="nearby-13-wrapper" style="margin:2px;width:15%;background-color: #25b53a" title="سبز">
                                    <br></div>
  
                                    <div id="nearby-7-wrapper" style="margin:2px;width:15%;background-color: #ffffff" title="سفید">
                                    <br></div>
          
                                    <div id="nearby-2-wrapper" style="margin:2px;width:15%;background-color: #c0c0c0" title="نقره ای">
                                    <br></div>
                                               </div>
                                    <div style="display: flex; margin: auto">

                                    <div id="nearby-17-wrapper" style="margin:2px;width:15%;background-color: #6f3e18" title="قهوه ای">
                                    <br></div>
                       
                                    <div id="nearby-11-wrapper" style="margin:2px;width:15%;background-color: #d4be8d" title="بژ">
                                    <br></div>
                  
                                    <div id="nearby-3-wrapper" style="margin:2px;width:15%;background-color: #808080" title="طوسی">
                                    <br></div>
                  
                                    <div id="nearby-62-wrapper" style="margin:2px;width:15%;background-color: #cdad00" title="طلایی">
                                    <br></div>
                  
                                    <div id="nearby-48-wrapper" style="margin:2px;width:15%;background-color: #ff6501" title="نارنجی">
                                    <br></div>
                         
                                    <div id="nearby-51-wrapper" style="margin:2px;width:15%;background-color: #657400" title="زیتونی">
                                    <br></div>
                                                               </div>
                                    <div style="display: flex; margin: auto">

                                    <div id="nearby-19-wrapper" style="margin:2px;width:15%;background-color: #ea0001" title="قرمز">
                                    <br></div>
                       
                                    <div id="nearby-41-wrapper" style="margin:2px;width:15%;background-color: #fffc00" title="زرد">
                                    <br></div>
                       
                                    <div id="nearby-54-wrapper" style="margin:2px;width:15%;background-color: #04ba94" title="سبز آبی">
                                    <br></div>
                     
                                    <div id="nearby-27-wrapper" style="margin:2px;width:15%;background-color: #800080" title="بنفش">
                                    <br></div>
                     
                                    <div id="nearby-72-wrapper" style="margin:2px;width:15%;background-color: #aarrggbb" title="بی رنگ">
                                    <br></div>
                     
                                    <div id="nearby-12-wrapper" style="margin:2px;width:15%;background-color: #ffe4c4" title="کرم">
                                    <br></div>
                                                      </div>
                                    <div style="display: flex; margin: auto">

                                    <div id="nearby-66-wrapper" style="margin:2px;width:15%;background-color: #a98307" title="عسلی">
                                    <br></div>
                         
                                    <div id="nearby-1-wrapper" style="margin:2px;width:15%;background-color: multicolor" title="چند رنگ">
                                    <br></div>
                         
                                    <div id="nearby-47-wrapper" style="margin:2px;width:15%;background-color: #800000" title="زرشکی">
                                    <br></div>
                 
                                    <div id="nearby-45-wrapper" style="margin:2px;width:15%;background-color: #ffc0cb" title="صورتی">
                                    <br></div>
                                                                        </div>

                                </span>
                            
</div>

</b-card>
</b-collapse>

    </div>
</template>
<script>
export default {
    
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
.collapsed > .when-opened,
:not(.collapsed) > .when-closed {
  display: none;
}
</style>
