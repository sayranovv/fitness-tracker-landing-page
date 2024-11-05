<script>
import AppPlanCard from "@/components/cards/AppPlanCard.vue";
export default {
  components: {AppPlanCard},
  setup() {
    return {
      plans: [
        {name: 'Free Plan', cost: 0, email: 5, share: 'Free Share', clients: 200, support: 'Chat support'},
        {name: 'Basic', cost: 5, email: 200, share: 'Free Share', clients: 500, support: 'Chat + Email support'},
        {name: 'Advanced', cost: 9, email: 2000, share: 'Free Share', clients: 1000, support: 'Chat + Email support'},
        {name: 'Most Advanced', cost: 12, email: 9999, share: 'Free Share', clients: 10000, support: 'Personal Manager'},
      ]
    }
  }
}
</script>

<template>
<div class="container">
  <div class="content">
    <p class="content-text">We have selected the best payment solutions for you.</p>
    <h3 class="content-title">Choose your tariff plan</h3>
  </div>
  <div class="buttons">
    <button class="btn btn-right">Month</button>
    <button class="btn btn-left">Years</button>
  </div>
  <div class="cards">

    <AppPlanCard
        v-for="plan in this.plans"
        :name="plan.name"
        :cost="plan.cost"
        :email="plan.email"
        :share="plan.share"
        :clients="plan.clients"
        :support="plan.support"
    />
  </div>
</div>
</template>

<style scoped>
.container {
  padding: 80px 120px;
}

.content-text {
  font-size: 18px;
  font-weight: 500;
  letter-spacing: 0.5px;
  text-align: center;
  color: #474A57;
}

.content-title {
  font-size: 45px;
  font-weight: 400;
  letter-spacing: 2px;
  font-family: "Permanent Marker", sans-serif;
  text-align: center;
  color: #1C1C1D;
  margin-top: 15px;
}

.buttons {
  margin-top: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.btn {
  padding: 15px 30px;
  border: 2px solid #1C1C1D;
  border-bottom: 5px solid #1C1C1D;
  font-size: 20px;
  font-weight: 700;
  letter-spacing: 0.6px;
  background-color: #fff;
}

.btn-right {
  border-bottom-left-radius: 23px;
  border-top-left-radius: 23px;
  border-right: 1px solid #1C1C1D;
}

.btn-right:active {
  border-bottom: 2px solid #1C1C1D;
}

.btn-left {
  border-bottom-right-radius: 23px;
  border-top-right-radius: 23px;
  border-left: 1px solid #1C1C1D;
}

.btn-left:active {
  border-bottom: 2px solid #1C1C1D;
}

.cards {
  margin-top: 52px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

@media (max-width: 768px) {
  .container {
    padding: 80px 30px;
  }

  .cards {
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
  }
}

@media (max-width: 1024px) and (min-width: 768px) {
  .container {
    padding: 80px 60px;
  }

  .cards {
    flex-wrap: wrap;
    justify-content: center;
    gap: 10px;
  }
}

@media (max-width: 1440px) and (min-width: 1024px) {
  .cards {
    flex-wrap: wrap;
    justify-content: center;
    gap: 10px;
  }
}


</style>