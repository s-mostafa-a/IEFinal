<template>
<div>
<div dir="rtl" style="display: flex">
<b-btn  variant="outline-success" v-b-toggle.collapse1 >
  <span class="when-opened">نام دسته -</span>
  <span class="when-closed">نام دسته +</span>
</b-btn>
</div>

  <b-collapse id="collapse1" class="mt-2">
          <b-card dir="rtl">

      <div>
      <b-btn v-b-toggle.collapse1_inner variant="outline-success" size="sm">نام دسته</b-btn>      
      <b-collapse id=collapse1_inner class="mt-2">
        <div>نام دسته</div>
        <div>نام دسته</div>
        <div>نام دسته</div>
        <div>نام دسته</div>
        <div>نام دسته</div>
      </b-collapse>
      </div>
      <div>

            <b-btn v-b-toggle.collapse1_inner1 variant="outline-success" size="sm">نام دسته</b-btn>      
      <b-collapse id=collapse1_inner1 class="mt-2">
        <div>نام دسته</div>
        <div>نام دسته</div>
        <div>نام دسته</div>
        <div>نام دسته</div>
        <div>نام دسته</div>
      </b-collapse>
      </div>
      <div>


            <b-btn v-b-toggle.collapse1_inner2 variant="outline-success" size="sm">نام دسته</b-btn>      
      <b-collapse id=collapse1_inner2 class="mt-2">
        <div>نام دسته</div>
        <div>نام دسته</div>
        <div>نام دسته</div>
        <div>نام دسته</div>
        <div>نام دسته</div>
      </b-collapse>
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
