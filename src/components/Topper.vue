<template>
  <div class="topper">
    <span class="left">
      <span class="material-icons unselectable">menu</span>
      <p class="unselectable">메뉴</p>
    </span>
    <span class="mid"
      ><img
        class="unselectable"
        src="https://rs.nxfs.nexon.com/gnb/images/logo_nexon.png"
        alt="logo"
    /></span>
    <span class="right unselectable">
      <span
        class="sign-up"
        @mouseover="mouseHovered.SignUp = true"
        @mouseleave="mouseHovered.SignUp = false"
        >회원가입</span
      >
      <span
        class="sign-in"
        @mouseover="mouseHovered.SignIn = true"
        @mouseleave="mouseHovered.SignIn = false"
        ><b>로그인</b></span
      >
    </span>
  </div>
</template>

<script>
export default {
  name: "Topper",
  data() {
    return {
      mouseHovered: {
        SignUp: false,
        SignIn: false,
      },
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
