<template>
  <div id="app" class="p-8 h-screen w-screen">
    <video
      class="absolute top-0 left-0 w-full h-full object-cover"
      autoplay
      loop
      muted
    >
      <source src="./assets/7btrrd.mp4" type="video/mp4" />
    </video>
    <div class="h-full w-full rounded-lg backdrop-blur-lg bg-base-100 bg-opacity-40">
      <top-bar-vue class="fixed" />
      <div class="grid grid-cols-10 h-full pt-20">
        <div class="col-span-2">
          <left-nav-vue class="h-full" />
        </div>
        <div class="col-span-8">
          <div class="h-full">1</div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import LeftNavVue from "./components/Basic/LeftNav.vue";
import TopBarVue from "./components/Basic/TopBar.vue";
export default {
  components: {
    TopBarVue,
    LeftNavVue,
  },
};
</script>
<style>
</style>
