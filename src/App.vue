<template>
  <div id="app" style="overflow: hidden">
    <MyHeader />
    <SectionOne />
    <SectionTwo />
    <SectionThree />
    <SectionFour />
    <SectionFive />
    <SectionSix />
    <SectionSeven />
    <SectionEight />
    <MyFooter /> -->
    <HelloWmyIntroduceorld msg="Welcome to Vue.js App" msg2="234" />
  </div>
</template>
<script>
import MyHeader from "./components/MyHeader.vue";
import SectionOne from "./components/SectionOne.vue";
import SectionTwo from "./components/SectionTwo.vue";
import SectionThree from "./components/SectionThree.vue";
import SectionFour from "./components/SectionFour.vue";
import SectionFive from "./components/SectionFive.vue";
import SectionSix from "./components/Section6.vue";
import SectionSeven from "./components/Section7.vue";
import SectionEight from "./components/Section8Fixed.vue";
import MyFooter from "./components/MyFooter.vue";
export default {
  name: "App",
  components: {
    MyHeader,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    SectionSix,
    SectionSeven,
    SectionEight,
    MyFooter,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  // margin-top: 60px;
}
// body {
//   margin: 0;
// }
</style>
