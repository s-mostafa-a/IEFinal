<template>
    <div>
        <my-button1 @clickedd="cleckHandler" />
        <div>
            {{myn}}
        </div>
        <MyButton @clickedd="cleckHandler" />

    </div>
</template>


<script>
import MyButton from '~/components/MyButton';
import MyButton1 from '~/components/MyButton1';

export default {
    props:['number'],
    components: {
        MyButton,
        MyButton1
    },
    data() {
        return {
            myn: this.number,
        }
    },
    methods: {
        cleckHandler: function(e) {
            alert(e);
            if(e == 1)
            this.myn -= 1;
            else
            this.myn += 1;

            
        }
    }
}
</script>

<style scoped>
</style>

