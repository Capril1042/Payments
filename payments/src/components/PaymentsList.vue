<template>
  <div>
  <table>
  <TableHeader></TableHeader>
  <tbody>
  <tr  v-for="payment in payments" v-bind:key="payment.id">
    <td>
      {{ payment.name }}
    </td>
    <td>
    {{ payment.ID}}
    </td>
    <td>
    {{ payment.description }}
    </td>
    <td>
    {{ payment.amount }}
    </td>
    </tr>
    </tbody>
    </table>
  </div>
</template>

<script>
import TableHeader from "./TableHeader.vue";
export default {
  name: "PaymentsList",
  components:{
    TableHeader
  },
  data() {
      return{
        payments: [
            {
                name: "name1",
                ID: "001A",
                description: "a description",
                amount: 50,
            
            },
             {
                name: "name2",
                ID: "001b",
                description: "another description",
                amount: 30
            },
        ],
      }
  }
}
</script>
