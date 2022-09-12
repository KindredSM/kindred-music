<template>
  <div class="home">
    <HelloWorld class="header" msg="" />
    <div class="links-container">
      <img src="@/assets/moth.webp" class="logo" alt="" srcset="" />
      <router-link to="/music" class="links"
        ><PageLinks msg="W.I.P Music"
      /></router-link>
      <router-link to="/gallery" class="links"
        ><PageLinks msg="Gallery"
      /></router-link>
      <a
        class="links"
        href="https://kindredsm.github.io/linkhub/"
        target="_blank"
      >
        <PageLinks msg="Linkhub"
      /></a>
      <a
        class="links"
        href="https://kindredsm.github.io/Cerebration/"
        target="_blank"
      >
        <PageLinks msg="Blog"
      /></a>
    </div>
  </div>
</template>

<style lang="scss">
.header {
  font-size: 1.5rem;
}

.logo {
  width: 80px;
  padding: 10px 0px 20px 0px;
}
</style>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import PageLinks from "/src/components/PageLinks.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
    PageLinks,
  },
};
</script>
