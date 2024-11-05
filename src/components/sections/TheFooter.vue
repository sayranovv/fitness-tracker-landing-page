<script>

</script>

<template>
<div class="container">
  <div class="logo">
    <img src="../../../public/assets/Big.png" alt="logo" class="logo-img">
  </div>
  <nav>
    <ul>
      <li>About</li>
      <li>Pricing</li>
      <li>Manual</li>
    </ul>
  </nav>
  <div class="buttons">
    <button class="btn-primary btn">
      <img src="../../../public/assets/appstore-white.png" alt="appstore icon">
      <span>Download</span>
    </button>
    <button class="btn-primary btn">
      <img src="../../../public/assets/playmarket-white.png" alt="playmarket icon">
      <span>Download</span>
    </button>
  </div>
</div>
</template>

<style scoped>
.container {
  padding: 40px 120px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #7711DD;
}

nav ul {
  display: flex;
  gap: 35px;
  list-style: none;
  font-size: 17px;
  font-weight: 700;
  letter-spacing: 0.5px;
}

.buttons {
  display: flex;
  justify-content: space-between;
  gap: 28px;
  align-items: center;
}

.btn {
  background-color: #FFBD12;
  padding: 11px 32px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  color: white;
}

.btn img {
  width: 25px;
}

@media (max-width: 768px) {
  .container {
    justify-content: center;
  }

  .logo {
    display: none;
  }

  nav ul {
    align-items: center;
  }

  .buttons {
    display: none;
  }
}

@media (max-width: 1024px) {
  .container {
    padding: 40px 60px;
  }
}

@media (max-width: 1200px) {
  .container {
    justify-content: center;
    gap: 50px;
  }

  .buttons {
    display: none;
  }
}
</style>