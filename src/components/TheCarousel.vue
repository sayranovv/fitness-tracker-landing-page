<script>
import {Swiper, SwiperSlide } from 'swiper/vue'
import 'swiper/css';
import AppCard from "@/components/cards/AppCard.vue";
export default {
  props: ['cards'],
  components: {AppCard, Swiper, SwiperSlide},
}
</script>

<template>
  <div class="container-caro">
    <Swiper class="carousel"
            :slides-per-view="5"
            :spaceBetween="30"
            loop
    >
      <SwiperSlide v-for="card in cards" :key="card.id">
        <AppCard :img="card.img" :title="card.title" :description="card.description" />
      </SwiperSlide>
    </Swiper>
  </div>
</template>

<style scoped>
.container-caro {
  width: 1800px;
  overflow: hidden;
}
.carousel {
  width: 100%;
}
</style>