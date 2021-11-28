<template>
  <Topper></Topper>
  <Banner></Banner>
</template>

<script>
import Topper from "@/components/Topper.vue";
import Banner from "@/components/Banner.vue";

export default {
  name: "App",
  components: { Topper, Banner },
  data() {
    return {};
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Material+Icons");
@font-face {
  font-family: "NEXON Lv1 Gothic OTF";
  src: url("https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_20-04@2.1/NEXON Lv1 Gothic OTF.woff")
    format("woff");
  font-weight: normal;
  font-style: normal;
}
@import "./assets/style.css";
.unselectable {
  user-select: none;
}
#app {
  font-family: "NEXON Lv1 Gothic OTF", "malgun gothic", "sans serif";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100vw;
  height: 100vh;
  padding: 0;
  margin: 0;
  overflow: hidden;
  display: flex;
  flex-direction: column;
}

body {
  width: 100vw;
  height: 100vh;
  padding: 0;
  margin: 0;
}
</style>
