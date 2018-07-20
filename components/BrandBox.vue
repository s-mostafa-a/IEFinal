<template>
<div>
<div dir="rtl" style="display: flex">
<b-btn  variant="outline-success" v-b-toggle.collapseb   style="width: 100%">
  <span class="when-opened">بر اساس برند -</span>
  <span class="when-closed">بر اساس برند +</span>
</b-btn>
</div>

  <b-collapse id="collapseb" class="mt-2">
          <b-card>
              <div>
                  <b-input placeholder="نام برند"/>
              </div>
            <div style="float: right">
            <b-checkbox title="1"> برند</b-checkbox>
            <hr>
                        <b-checkbox title="1"> برند</b-checkbox>
            <hr>
                        <b-checkbox title="1"> برند</b-checkbox>
            <hr>
                        <b-checkbox title="1"> برند</b-checkbox>
            <hr>
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
