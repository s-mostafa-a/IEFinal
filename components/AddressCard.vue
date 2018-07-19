<template>
    <div>
        <b-table 
             bordered="true"
             fixed="true"
             :items="items">
    </b-table>
    </div>
</template>

<script>
export default {
    props: ['selected'],
    data(){
        return{
            name: 'نام',
        items: [
        { 1:"تحویل گیرنده: " ,2:'Dickerson', 3:'Macdonald' },
      ],
        }
    }
    
}
</script>
<style scoped>

</style>
