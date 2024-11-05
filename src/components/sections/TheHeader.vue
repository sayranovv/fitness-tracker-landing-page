<script>
</script>

<template>
  <header class="container">
    <div class="header-content">
      <h1 class="header-content-title">The best<br>fitness tracker!</h1>
      <p class="header-content-text">
        Nisi ullamco tempor tempor nulla labore ad labore sit eu duis. Ut et esse cupidatat consequat ea exercitation.
      </p>
      <div class="buttons">
        <button class="btn-primary btn">
          <img src="../../../public/assets/appstore-black.png" alt="appstore icon">
          <span>Download</span>
        </button>
        <button class="btn-primary btn">
          <img src="../../../public/assets/playmarket-black.png" alt="playmarket icon">
          <span>Download</span>
        </button>
      </div>
    </div>
    <div class="header-image">
      <img src="../../../public/assets/Illustration.png" alt="header-image" class="header-image-img">
    </div>
  </header>
</template>

<style scoped>
.container {
  max-width: 1440px;
  width: 100%;
  padding: 0 120px;
  background-color: #7711DD;
  display: flex;
  position: relative;
  justify-content: space-between;
}

.header-content {
  padding-top: 160px;
  padding-bottom: 265px;
  max-width: 590px;
  width: 100%;
}

.header-content-title {
  font-family: "Permanent Marker", cursive;
  font-weight: 400;
  font-style: normal;
  font-size: 70px;
  letter-spacing: 2px;
  line-height: 75.5px;
}

.header-content-text {
  margin-top: 30px;
  max-width: 420px;
  width: 100%;
  font-size: 18px;
  font-weight: 200;
}

.buttons {
  display: flex;
  gap: 15px;
  align-items: center;
}

.btn {
  background-color: #fff;
  padding: 11px 32px;
  margin-top: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  color: #1C1C1D;
}

.btn:hover {
  background-color: #1BDBC4;
}

.btn:active {
  border-bottom: 2px solid #1C1C1D;
}

.btn img {
  width: 25px;
}

.header-image {
  position: absolute;
  overflow: hidden;
  left: 640px;
  top: -29px;
}

.header-image-img {
  max-width: 800px;
}

@media (max-width: 768px) {
  .container {
    padding: 0 30px;
    justify-content: center;
  }

  .header-content {
    max-width: 400px;
  }
  .header-image {
    display: none;
  }

  .buttons {
    justify-content: space-between;
  }

  .btn {
    width: 100%;
    padding: 15px 15px;
    flex-direction: column;
    flex-wrap: wrap;
    justify-content: center;
  }
}

@media (max-width: 1024px) {
  .container {
    padding: 0 60px;
  }

  .header-image {
    display: none;
  }
}

@media (max-width: 1200px) {
  .header-image {
    display: none;
  }
}

@media (max-width: 1440px) {
  .container {
    position: static;
    align-items: center;
  }

  .header-content {
    padding-bottom: 67px;
  }

  .header-image {
    position: absolute;
    left: 50%;
    top: 10%;
    width: 600px;
  }
  .header-image img {
    display: block;
    width: 100%;
    height: auto;
  }
}

</style>