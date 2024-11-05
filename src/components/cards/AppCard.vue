<script>
export default {
  props: ['key', 'img', 'title', 'description'],
}
</script>

<template>
<div class="card">
  <div class="content">
    <div class="card-image">
      <img src="../../../public/assets/Group%2015.png" alt="card-image" class="template-card-image">
    </div>
    <div class="card-title">
      {{ this.title }}
    </div>
  </div>
  <div class="description">
    {{ this.description }}
  </div>
</div>
</template>

<style scoped>
.card {
  width: 340px;
  border-radius: 10px;
  border: 2px solid #1C1C1D;
  border-bottom: 5px solid #1C1C1D;
  background-color: #FFB0BC;
}

.content {
  display: flex;
  gap: 25px;
  margin: 25px 20px 15px 20px;
}

.card-image {
  border: 2px solid #1C1C1D;
  border-radius: 10px;
  background-color: #fff;
  width: 87px;
  height: 73px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.card-title {
  width: 173px;
  font-size: 20px;
  font-weight: 700;
}

.description {
  padding: 0 20px 20px 20px;
  font-size: 16px;
  font-weight: 400;
}
</style>