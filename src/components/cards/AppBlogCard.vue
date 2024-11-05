<script>
export default {
  props: ['color']
}
</script>

<template>
<div class="card-container">
  <div :class="'card-image-' + this.color">
    <img src="../../../public/assets/Group%2015.png" alt="template-img">
  </div>
  <h4 class="card-title">Stories of our users</h4>
  <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  <p class="card-date">17.10.24</p>
</div>
</template>

<style scoped>
.card-container {
  max-width: 380px;
  width: 100%;

}

.card-image-cyan {
  width: 100%;
  height: 260px;
  display: flex;
  justify-content: center;
  align-items: center;
  border: 2px solid #1C1C1D;
  border-bottom: 9px solid #1C1C1D;
  border-radius: 10px;
  background-color: #1BDBC4;
}

.card-image-purple {
  width: 100%;
  height: 260px;
  display: flex;
  justify-content: center;
  align-items: center;
  border: 2px solid #1C1C1D;
  border-bottom: 9px solid #1C1C1D;
  border-radius: 10px;
  background-color: #962EFF;
}

.card-title {
  color: #1C1C1D;
  font-size: 24px;
  font-weight: 700;
  letter-spacing: 0.6px;
  margin-top: 20px;
}

.card-text {
  color: #474A57;
  font-size: 18px;
  font-weight: 400;
  letter-spacing: 0.5px;
  margin-top: 9px;
}

.card-date {
  color: #1C1C1D;
  font-size: 18px;
  font-weight: 500;
  letter-spacing: 0.5px;
  margin-top: 18px;
}
</style>