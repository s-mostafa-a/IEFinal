<template>
<div>
<b-container fluid class="p-4 ">
<b-table striped :fields="fields" :items="items" dir="rtl" >
    <template slot="details" slot-scope="data">
    <b-btn v-b-toggle.myCollapse variant="primary">>></b-btn>
    </template>

</b-table>

        <b-collapse id="myCollapse">
                    <buy-basket />
        </b-collapse>

      </b-container>

</div>
</template>
<script>
import BuyBasket from '~/components/BuyBasket.vue'
export default {
    components:{
        BuyBasket,
    },
    data() {
    return {
      fields: [
        {
          key: "index",
          label: "ردیف",
          formatter: (value) => { return value }
        },
        {
          key: "code",
          label: "کد",
          formatter: (value) => { return value }
        },
        {
          key: "date",
          label: "تاریخ و ساعت",
          formatter: (value) => { return value }
        },
        {
          key: "price",
          label: "مبلغ کل",
          formatter: (value) => { return value }
        },
        {
          key: "status",
          label: "وضعیت",
          formatter: (value) => { return value }
        },
        {
          key: "action",
          label: "عملیات",
          formatter: (value) => { return value }
        },
        {key: "details",
          label: "جزییات",
          formatter: (value) => { return value }
        }
      ],
      items: [
        {index: 1,
        code: 'code',
        date: 'date',
        price: 'price',
        status: 'status',
        action: 'action',
        details: ' '
        },
        {index: 1,
        code: 'code',
        date: 'date',
        price: 'price',
        status: 'status',
        action: 'action',
        details: ' '
        },
        {index: 1,
        code: 'code',
        date: 'date',
        price: 'price',
        status: 'status',
        action: 'action',
        details: ' '
        },
        
      ]
    };
  },
}
</script>

<style scoped>

</style>
