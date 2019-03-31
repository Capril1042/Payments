<template>
  <div>
    <div v-for="payment in payments">{{ payment.name }}</div>
  </div>
</template>

<script>
export default {
name: "PaymentsList",
    data() {
        return {
            payments: [
                {
                    name: "name 1",
                },
                {
                    name: "name 2",
                }]
    };
    }
    };
</script>
