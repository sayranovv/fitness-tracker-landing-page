<script>

</script>

<template>
<div class="container">
  <div class="content">
    <h2 class="content-header">Start training already on your watch</h2>
    <p class="content-text">Nisi ullamco tempor tempor nulla labore ad labore sit eu duis. Ut et esse cupidatat consequat. Nisi ullamco tempor tempor nulla labore ad labore sit eu duis. Ut et esse cupidatat consequat.</p>
    <form action="#" class="content-form">
      <input type="text" class="content-form-input" placeholder="Email" />
      <button class="btn-primary yellow">Let's GO!</button>
    </form>
  </div>
  <div class="watch-image">
    <img src="../../../public/assets/watch.png" alt="watch" class="watch-image-img">
  </div>
</div>
</template>

<style scoped>
.container {
  padding: 0 120px;
  background-color: #962EFF;
  display: flex;
  align-items: center;
  gap: 117px;
}

.content {
  padding-top: 164px;
  padding-bottom: 164px;
  max-width: 484px;
}

.content-header {
  font-family: "Permanent Marker", sans-serif;
  font-size: 45px;
  font-weight: 400;
  letter-spacing: 2px;
  line-height: 48.5px;
}

.content-text {
  margin-top: 25px;
  font-size: 18px;
  font-weight: 400;
  line-height: 27px;
  letter-spacing: 0.5px;
}

.content-form {
  margin-top: 50px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.content-form-input {
  font-family: "Montserrat", sans-serif;
  font-size: 18px;
  font-weight: 500;
  line-height: 26px;
  letter-spacing: 0.5px;
  max-width: 277px !important;
  width: 100%;
  padding: 10px 20px;
  border: 1px solid #1C1C1D;
  border-bottom: 3px solid #1C1C1D;
  border-radius: 10px;
}

.yellow {
  background-color: #FFBD12;
  color: #fff;
  max-width: 190px;
  width: 100%;
  padding: 12px;
}

.yellow:active {
  border-bottom: 2px solid #1C1C1D;
}

.watch-image {
  padding-top: 50px;
  width: 600px;
}

.watch-image-img {
  width: 100%;
}

@media (max-width: 768px) {
  .container {
    padding: 0 30px;
    justify-content: center;
  }

  .watch-image {
    display: none;
  }

  .content-form {
    flex-wrap: wrap;
    flex-direction: column;
    gap: 15px;
  }

  .content-form-input {
    max-width: 100% !important;
    width: 100%;
  }

  .yellow {
    height: 50px;
    background-color: #FFBD12;
    color: #fff;
    max-width: 100% !important;
    width: 100%;
  }
}

@media (max-width: 1024px) and (min-width: 768px) {
  .container {
    padding: 0 60px;
    gap: 20px;
  }
}

</style>