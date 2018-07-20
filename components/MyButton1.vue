<template>
    <button   v-on:click="inputHandler"
                class="tajrobe" >+</button>
    
</template>

<script>
export default {
    data() {
        return {
        }
    },
    methods: {
        inputHandler: function(event){
            // console.log(event);
            this.$emit('clickedd', 2);
                // console.log(event.target.value); 
            // this.$emit('searched', event);
        }
    } 
}
</script>


<style scoped>
.tajrobe{
    font-size: 100%;
    border: 1px solid black;
    border-radius: 25px;
    color: #ffffff;
    -webkit-transition: background-color 0.4s ease;
    transition: background-color 0.4s ease;
    background-color: dimgray;
}
</style>
