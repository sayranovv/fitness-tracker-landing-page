<template>
  <TheNavbar />
  <TheHeader />
  <TheInfo />
  <TheCallToAction />
  <TheBlog />
  <ThePrices />
  <TheForm />
  <TheFooter />
</template>

<script>
import TheHeader from '@/components/sections/TheHeader.vue'
import TheNavbar from '@/components/TheNavbar.vue'
import TheInfo from '@/components/sections/TheInfo.vue'
import TheCallToAction from "@/components/sections/TheCallToAction.vue";
import TheBlog from "@/components/sections/TheBlog.vue";
import TheForm from "@/components/sections/TheForm.vue";
import TheFooter from "@/components/sections/TheFooter.vue";
import ThePrices from "@/components/sections/ThePrices.vue";

export default {
  name: 'App',
  components: {
    ThePrices,
    TheHeader, TheInfo, TheCallToAction, TheBlog, TheForm, TheFooter, TheNavbar
  }
}
</script>

<style>
#app {
  margin: 0 auto;
  color: #fff;
  font-family: "Montserrat", sans-serif;
  font-weight: 400;
}
</style>
