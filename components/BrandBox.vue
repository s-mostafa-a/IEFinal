<template>
    <div >  
        <b-card>
<b-btn v-b-toggle.Collapse1>
  <span class="when-opened">Close</span>
  <span class="when-closed">Open</span>
  My Collapse
</b-btn>
<div id="Collapse1" >
        <p class="card-text">
            Some quick example text to build on the <em>card title</em> and make up the bulk of the card's content.
        </p>
        <a href="#"
           class="card-link">Card link</a>
        <b-link href="#"
                class="card-link">Another link</b-link>
</div>
        </b-card>
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
