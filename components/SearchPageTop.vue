<template>
    <div style="display: flex;margin:auto;">
        <div>
        مرتب‌سازی بر اساس:
        </div>
        <div>
    <b-dropdown id="ddown1" variant="link" text="محبوبترین" size="sm">
            <b-dropdown-item>گرانترین</b-dropdown-item>
            <b-dropdown-item>ارزانترین</b-dropdown-item>
            <b-dropdown-item>مرتبط‌ترین</b-dropdown-item>
        </b-dropdown>
        </div>
        	&nbsp;

                                	&nbsp;
                                    	&nbsp;	&nbsp;
                                        	&nbsp;
                                            	&nbsp;
                                                	&nbsp;	&nbsp;	&nbsp;	&nbsp;	&nbsp;	&nbsp;	&nbsp;	&nbsp;	&nbsp;	&nbsp;
        <div >

            <b-pagination  size="md" :total-rows="100" v-model="currentPage" :per-page="10">
    </b-pagination>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            page_no: 1,
            page_max: 10
        }
    },
    methods:{
        inc: function(){
            page_no += 2;
            page_no %= 10;
            alert(6)
        },
        dec: function(){
            page_no -= 1;
            page_no %= 10;
        }
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
</style>
