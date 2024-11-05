<script>
export default {
  props: ['name', 'cost', 'email', 'share', 'clients', 'support']
}
</script>

<template>
<div :class="'card-container' + ' v-' + cost">
  <p class="plan">{{ name }}</p>
  <p class="cost">${{ cost }} mounth</p>
  <ul class="description">
    <li v-if="email !== 9999">{{ email }} Email</li>
    <li v-else>Unlim Email</li>
    <li>{{ share }}</li>
    <li>{{ clients }} Clients</li>
    <li>{{ support }}</li>
  </ul>
  <button class="btn-primary btn-card">Get started</button>
</div>
</template>

<style scoped>
.card-container {
  max-width: 278px;
  width: 100%;
  padding: 30px 30px 40px 30px;
  background-color: #F95A2C;
  border: 2px solid #1C1C1D;
  border-bottom: 8px solid #1C1C1D;
  border-radius: 10px;
  color: #1C1C1D;
  letter-spacing: 0.5px;
}

.v-0 {
  background-color: #F95A2C;
}

.v-5 {
  background-color: #1BDBC4;
}

.v-9 {
  background-color: #962EFF;
}

.v-12 {
  background-color: #FFBD12;
}

.plan {
  font-size: 18px;
  font-weight: 500;
}

.cost {
  margin-top: 20px;
  font-size: 30px;
  font-weight: 600;
  line-height: 45px;
}

.description {
  margin-top: 30px;
  list-style: none;
  font-size: 18px;
  font-weight: 500;
  line-height: 26px;
}

.description li {
  margin-top: 10px;
}

.btn-card {
  margin-top: 30px;
  width: 100%;
  padding: 17px;
}
</style>