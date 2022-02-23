<template>
  <div>
    <Header :fastName="fName" @updateValue="fName = $event" />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header_footer/Header.vue";
import Footer from "./components/Header_footer/Footer.vue";
export default {
  data() {
    return {
      fName: "jhon",
      lName: "doe",
      age: 56,
    };
  },
  components: {
    Header,
    Footer,
  },
};
</script>
<style>
.myAge {
  color: red;
}
.hello:hover {
  font-weight: 900;
  color: palevioletred;
  animation: all;
}
body {
  font-family: "Roboto", sans-serif;
}
</style>
