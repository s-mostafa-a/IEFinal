<template>
<div>
<b-container fluid class="p-4 ">
<b-table striped :fields="fields" :items="items" dir="rtl" >
    <template slot="mosh" slot-scope="data">
        <div style="display: flex;margin: auto;text-align:center;">
            <div>
                    <img :src="data.value.pic" width="80px" height="80px"/>
            </div>
            <div style="font-size: 10px">
                <div style="font-size: 15px">
              {{data.value.brand}}
              </div>
               <div> 
                {{data.value.name}}
                            </div>
               <div> 
              {{data.value.color}}
                            </div>
               <div> 
              {{data.value.size}}
                            </div>
               <div> 
              {{data.value.code}}
                            </div>
              </div>
        </div>
    </template>
    <template slot="ted" slot-scope="data">
        <incer :number=1 />
    </template>
    <template slot="gh" slot-scope="data">
        <div>
              {{data.value.price}}<br>
              {{data.value.off}}<hr>
              {{data.value.final}}

        </div>

    </template>
        <!--template slot="mosh" slot-scope="data">
            <img :src="data.mosh.pic" width="80px" height="80px"/>
    </template-->
</b-table>

      </b-container>

</div>
</template>
<script>
import Incer from '~/components/Incer.vue'
export default {
    components:{
        Incer,
    },
  data() {
    return {
      fields: [
        {
          key: "index",
          label: "ردیف",
          formatter: "indexer"
        },
        {
          key: "mosh",
          label: "مشخصات",
          formatter: "mosher"
        },
        {
          key: "ted",
          label: "تعداد",
          formatter: "teder"
        },
        {
          key: "gh",
          label: "قیمت",
          formatter: "gher"
        }
      ],
      items: [
        {index: 1,
          mosh: {
            pic: "URL",
            brand: "Doe",
            name: "name",
            color: "color",
            size: "size",
            code: "code"
          },
          ted: 1,
          gh: { price: "price", off: "off", final: "final" }
        },        
        {index: 2,
          mosh: {
            pic: "URL",
            brand: "Doe",
            name: "name",
            color: "color",
            size: "size",
            code: "code"
          },
          ted: 1,
          gh: { price: "price", off: "off", final: "final" }
        }
        
      ]
    };
  },
  methods: {
    dec: function(inde) {
        for(var i in this.items){
            if(i.index == inde){
                if(i.ted > 0)
                    i.ted -= 1;
            }
        }
              

    },
    inc: function(inde) {
        for(var i in this.items.value){
            console.log(i.index)
        }
    },
    indexer: function(value) {
      return value;
    },
    mosher: function(value) {
      return value;
    },
    teder: function(value) {
      return value;
    },
    gher: function(value) {
      return value;
    }
  }
};
</script>

<style scoped>
@font-face {
  font-family: "my_iran_sans";
  src: url("./fonts/IRAN-sans.ttf");
}

* {
  font-family: "my_iran_sans";
}

.tajrobe {
  float: left;
  font-size: 100%;
  border: 1px solid #6464ff;
  border-radius: 25px;
  width: 15%;
  color: #ffffff;
  -webkit-transition: background-color 0.4s ease;
  transition: background-color 0.4s ease;
  background-color: #3232ff;
}
#brow {
  background-color: gray;
  color: white;
}
#brow2 {
  background-color: white;
  color: black;
}
.gerd {
  font-size: 100%;
  border: 1px solid #6464ff;
  border-radius: 50px;
  width: 10%;
  color: #ffffff;
  -webkit-transition: background-color 0.4s ease;
  transition: background-color 0.4s ease;
  background-color: #3232ff;
}
</style>
