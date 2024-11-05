<script>
import AppBlogCard from "@/components/cards/AppBlogCard.vue";

export default {
  components: {AppBlogCard},
}
</script>

<template>
<div class="container">
  <h3 class="h3">Stories of our users</h3>
  <div class="cards">
    <AppBlogCard :color="'cyan'"/>
    <AppBlogCard :color="'purple'"/>
    <AppBlogCard :color="'cyan'"/>
  </div>
</div>
</template>

<style scoped>
.container {
  padding: 150px 120px 120px 120px;
}

.h3 {
  color: #1C1C1D;
  font-family: "Permanent Marker", sans-serif;
  font-size: 45px;
  font-weight: 400;
  letter-spacing: 2px;
  text-align: center;
}

.cards {
  margin-top: 60px;
  display: flex;
  flex-wrap: nowrap;
  justify-content: space-between;
  align-items: center;
}

@media (max-width: 768px) {
  .container {
    padding: 150px 30px 120px 30px;
  }

  .cards {
    flex-direction: column;
    gap: 40px;
  }
}

@media (max-width: 1024px) and (min-width: 768px) {
  .container {
    padding: 150px 60px 120px 60px;
  }

  .cards {
    gap: 20px;
  }
}

@media (max-width: 1440px) and (min-width: 1024px) {
  .cards {
    gap: 20px;
  }
}
</style>