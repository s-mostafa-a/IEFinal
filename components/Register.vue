
        <template>
            
        <b-modal hide-footer id="ozviat"
                    centered
                    ref="modal"
                    title="عضویت" style="text-align:center">
            <form>
                <p id="title"> شماره تلفن یا ایمیل </p>
                <b-form-input id= "input"
                            type="text"
                            placeholder="برای مثال parham.yassini@gmail.com"
                            v-model="name1">
                </b-form-input>
                <p id="title"> رمز عبور</p>             
                <b-form-input id= "input"
                            type="text"
                            placeholder=""
                            v-model="pass1">
                </b-form-input>
            </form>
            <b-btn id="register">ثبت نام</b-btn> 
        </b-modal>
        </template>
        <style scoped>
        @font-face {
    font-family: "my_iran_sans";
    src: url("./fonts/IRAN-sans.ttf");
}

* {
    font-family: "my_iran_sans";
}
        .reg {
        flex: 2 0 auto;
	    display: flex;
        float: right; 
        margin-right: 50px;
        
    }
    .button {
        border-radius: 20px; 
        width: 100%; 
        height: 40%;
    }
    #v {
        flex: 1 0 auto;
        border-color:  rgb(112,112,112);
        font-family: myFirstFont;
        background-color: rgb(112,112,112); 
        color: white;
    }
    #o {
        flex: 1 0 auto;
        font-family: myFirstFont;
        background-color: white;
        color: darkgray;
        margin-left: 2px;
    }
    #v:hover {
        
        flex: 1 0 auto;
        border-color:#006DF0;
        font-family: myFirstFont;
        color: white;
        background-color: #006DF0; 
        color:white;
    }
    #o:hover {
        flex: 1 0 auto;
        background-color:white;
        font-family: myFirstFont; 
        color:#006DF0; 
        border-color:#006DF0;
    }
    #modalPrevent {
        font-family: myFirstFont; 
        text-align: center;
    }
    #input {
        font-family: myFirstFont;
        border-radius: 14px;
        width: 80%;
        height: 60%;
        border-style: solid;
        border-color:  rgb(112,112,112);
        color: darkgray;
        text-align: right;
        padding-right: 8px;
    }
    #title {
        font-family: myFirstFont; 
        text-align: right;
        color: #006DF0;
    }
    #forget {
        font-family: myFirstFont;
        text-align: center;
    }
    #forget > a {
        color: #006DF0;
    }
    #enter {
        font-family: myFirstFont; 
        border-radius: 20px;
        width: 150px;
        margin-left: 50%;
        margin-right: 50%;
    }
    #register {
        font-family: myFirstFont;
    }
        </style>
        
        