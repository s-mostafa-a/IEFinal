<template>
    <button   v-on:click="inputHandler"
                 >+</button>
    
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

</style>
