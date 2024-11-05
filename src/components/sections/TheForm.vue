<script>
import TheCheckbox from '../TheCheckbox.vue'

export default {
  components: {TheCheckbox}
}
</script>

<template>
<div class="container">
  <div class="content">
    <h3 class="content-title">Download now and get a bonus!</h3>
    <p class="content-text">Nisi ullamco tempor tempor nulla labore ad labore sit eu duis. Ut et esse cupidatat consequat ea exercitation.</p>
    <div class="content-buttons">
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
  <div class="form-container">
    <div class="switcher">
      <a class="signin" href="#">Sign in</a>
      <a class="login" href="#">Log in</a>
    </div>
    <form action="#" class="form">
      <input type="text" class="form-input" placeholder="Your name" />
      <input type="text" class="form-input" placeholder="Email" />
      <input type="text" class="form-input" placeholder="Company" />
<!--      <div class="checkbox">-->
<!--        <input type="checkbox" class="form-checkbox" id="check">-->
<!--        <label for="check">sdfdsfsd</label>-->
<!--      </div>-->
      <div class="checkbox">
        <TheCheckbox />
        <span>Lorem ipsum dolor sit amet.</span>
      </div>
      <button class="btn-primary form-btn">Sign in</button>
    </form>
  </div>
</div>
</template>

<style scoped>
.container {
  padding: 80px 120px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.content {
  max-width: 400px;
  width: 100%;
}

.content-title {
  font-family: "Permanent Marker", sans-serif;
  font-size: 45px;
  font-weight: 400;
  letter-spacing: 2px;
  line-height: 48.5px;
  color: #1C1C1D;
}

.content-text {
  margin-top: 25px;
  font-size: 18px;
  font-weight: 400;
  line-height: 27px;
  letter-spacing: 0.5px;
  color: #474A57;
}

.content-buttons {
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
  margin-top: 50px;
}

.btn {
  background-color: #FA6648;
  padding: 11px 32px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  color: white;
}

.btn:active {
  border-bottom: 2px solid #1C1C1D;
}

.btn img {
  width: 25px;
}

.form-container {
  margin-right: 100px;
  max-width: 480px;
  border: 2px solid #1C1C1D;
  border-bottom: 5px solid #1C1C1D;
  border-radius: 10px;
  padding: 40px;
}

.switcher {
  font-size: 24px;
  font-weight: 700;
  line-height: 32px;
  letter-spacing: 0.6px;
}

.signin {
  text-decoration: none;
  color: #FA6648;
}

.login {
  margin-left: 20px;
  text-decoration: none;
  color: #1C1C1D;
}

.form {
  margin-top: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 15px;
}

.form-input {
  width: 403px;
  border: 1px solid #1C1C1D;
  border-bottom: 3px solid #1C1C1D;
  border-radius: 10px;
  padding: 13px 20px;
  font-family: "Montserrat", sans-serif;
  font-size: 18px;
  font-weight: 500;
  letter-spacing: 0.5px;
  color: #1C1C1D;
}

.checkbox {
  margin-top: 20px;
  width: 100%;
  color: #474A57;
  font-weight: 500;
  font-size: 18px;
  letter-spacing: 0.5px;
  display: flex;
  gap: 15px;
}

.checkbox span {
  margin-top: 4px;
}

.form-btn {
  margin-top: 30px;
  color: white;
  width: 100%;
  padding: 15px;
  background-color: #FA6648;
  font-weight: 900;
  font-size: 16px;
  letter-spacing: 0.5px;
}

.form-btn:active {
  margin-top: 33px;
  border-bottom: 2px solid #1C1C1D;
}

@media (max-width: 768px) {
  .container {
    padding: 80px 30px;
    display: flex;
    gap: 90px;
    align-items: center;
    flex-direction: column;
    flex-wrap: wrap;
  }

  .content-buttons {
    width: 100%;
    gap: 20px;
  }

  .btn {
    padding: 15px 15px;
    flex-direction: column;
    flex-wrap: wrap;
    justify-content: center;
  }

  .switcher {
    text-align: center;
  }

  .form-container {
    margin-right: 0;
    width: 100%;
  }

  .form-input {
    max-width: 100% !important;
  }

  .checkbox span {
    margin-top: 0;
  }

  .btn {
    width: 100%;
    flex-wrap: wrap;
  }
}

@media (max-width: 1200px) and (min-width: 768px) {
  .container {
    padding: 80px 60px;
    gap: 40px;
    flex-wrap: wrap;
    justify-content: center;
  }

  .form-container {
    margin-right: 0;
    width: 100%;
  }
}

@media (max-width: 1440px) {
  .form-container {
    margin-right: 0;
    width: 100%;
  }
}
</style>