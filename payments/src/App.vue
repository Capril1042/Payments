<template>
<div id="app" class="container">
  <PaymentsList></PaymentsList>
  </div>
</template>

<script>
import PaymentsList from "./components/PaymentsList.vue";

export default {
  name: "app",
  components: {
    PaymentsList
  }
};
</script>

<style>
* {
  box-sizing: border-box;
}
.container {
  max-width: 600px;
  margin: 0 auto;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  font-size: 30px;
}
</style>
