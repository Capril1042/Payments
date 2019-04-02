<template>
  <thead>
    <tr>
    <th v-for="col in columns" v-bind:key="col">
      {{ col }}
      </th>
    </tr>
  </thead>
</template>

<script>

export default {
  name: "TableHeader",
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
  },
  computed: {
      columns: function () {
          return Object.keys(this.payments[0]);
      }
          
      }
  }
</script>

<style>
thead {
    background: #99ffcc;
}

tr {
    text-align: left;
    padding:5%;
    font-size: 30px;
}
</style>