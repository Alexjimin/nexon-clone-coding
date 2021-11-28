<template>
  <div class="banner">
    <div class="banner-content-container">
      <div class="banner-content">
        <img v-bind:src="BannerImages[BannerPosition]" alt="a" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Banner",
  data() {
    return {
      BannerPosition: 0,
      BannerImages: [
        "https://rs.nxfs.nexon.com/bannerusr/21/11/C7x117154551704.png",
        "https://rs.nxfs.nexon.com/bannerusr/21/11/24JL25105114402.jpg",
        "https://rs.nxfs.nexon.com/bannerusr/21/11/wc8j25173925006.png",
        "https://rs.nxfs.nexon.com/bannerusr/21/11/hZtP25115339941.png",
        "https://rs.nxfs.nexon.com/bannerusr/21/11/WVF824175510292.jpg",
        "https://rs.nxfs.nexon.com/bannerusr/21/11/LeTC22093916848.png",
        "https://rs.nxfs.nexon.com/bannerusr/21/11/L1By25131511602.jpg",
        "https://rs.nxfs.nexon.com/bannerusr/21/11/24JL25105114402.jpg",
      ],
      SetBannerPosition: window.setInterval(() => {
        this.BannerPosition += 1;
        this.BannerPosition = this.BannerPosition % this.BannerImages.length;
        console.log(1);
      }, 10000),
    };
  },
};
</script>

<style scoped>
</style>