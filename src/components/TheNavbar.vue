<script>

</script>

<template>
<nav class="navbar">
  <a href="#" class="logo-link">
    <img src="../../public/assets/Big.png" alt="Logo" class="logo">
  </a>
  <div class="right-elements">
    <div class="nav-socials">
      <a href="#" class="nav-social">
        <img src="../../public/assets/Facebook.png" alt="Facebook" class="nav-social-logo">
      </a>
      <a href="#" class="nav-social">
        <img src="../../public/assets/Linkedin.png" alt="LinkedIn" class="nav-social-logo">
      </a>
      <a href="#" class="nav-social">
        <img src="../../public/assets/Google.png" alt="Google" class="nav-social-logo">
      </a>
    </div>
    <a href="#" class="burger-menu-link">
      <img src="../../public/assets/Menu.png" alt="Menu" class="burger-menu-logo">
    </a>
  </div>
</nav>
</template>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1440px;
  width: 100%;
  background-color: #7711DD;
  padding: 0 120px;
  height: 90px;
}

.right-elements {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 50px;
}

.nav-socials {
  display: flex;
  gap: 22px;
}

@media (max-width: 768px) {
  .navbar {
    padding: 0 30px;
    height: 100px;
  }

  .burger-menu-link {
    margin-left: 35px;
  }
}
</style>