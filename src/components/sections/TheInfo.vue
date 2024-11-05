<script>
import AppCard from "@/components/cards/AppCard.vue";
export default {
  components: {AppCard},
  setup() {
    return {
      cards: [
          {id: 0, img: '../../../public/assets/Group%2015.png', title: 'Nisi ullamco tempor tempor nulla.', description: 'Nisi ullamco tempor tempor nulla labore ad labore sit eu duis.'},
          {id: 1, img: '../../../public/assets/Group%2015.png', title: 'Nisi ullamco tempor tempor nulla.', description: 'Nisi ullamco tempor tempor nulla labore ad labore sit eu duis.'},
          {id: 2, img: '../../../public/assets/Group%2015.png', title: 'Nisi ullamco tempor tempor nulla.', description: 'Nisi ullamco tempor tempor nulla labore ad labore sit eu duis.'},
          {id: 3, img: '../../../public/assets/Group%2015.png', title: 'Nisi ullamco tempor tempor nulla.', description: 'Nisi ullamco tempor tempor nulla labore ad labore sit eu duis.'},
          {id: 4, img: '../../../public/assets/Group%2015.png', title: 'Nisi ullamco tempor tempor nulla.', description: 'Nisi ullamco tempor tempor nulla labore ad labore sit eu duis.'},
      ]
    }
  }
}
</script>

<template>
  <div class="container">
    <div class="content">
      <h2 class="content-header">About text</h2>
      <p class="content-text">Nisi ullamco tempor tempor nulla labore ad labore sit eu duis. Ut et esse cupidatat consequat.</p>
    </div>
    <div class="cards">
      <AppCard v-for="card in cards" :key="card.id" :img="card.img" :title="card.title" :description="card.description" />
    </div>
    <div class="switcher">
      <img src="../../../public/assets/Small.png" alt="switcher">
    </div>
  </div>
</template>

<style scoped>
.container {
  padding: 80px 0;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  overflow: hidden;
}

.content {
  text-align: center;
}

.content-header {
  font-family: "Permanent Marker", sans-serif;
  color: #1C1C1D;
  font-size: 45px;
  font-weight: 400;
}

.content-text {
  margin-top: 30px;
  color: #1C1C1D;
  font-size: 18px;
  font-weight: 400;
  max-width: 500px;
}

.cards {
  margin-top: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
}

.switcher {
  margin-top: 50px;
}

@media (max-width: 768px) {
  .container {
    padding: 80px 30px;
  }
}
</style>