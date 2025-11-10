<template>
  <div class="welcome-banner">
    <img
      src="https://res.cloudinary.com/demo/image/upload/v1720000000/urbilux-banner.jpg"
      alt="Welcome to Urbilux"
      class="banner-image"
    />

    <div class="banner-content">
      <h1 class="banner-title">Welcome to <span>Urbilux</span></h1>
      <p class="banner-subtitle">
        Discover the latest trends in fashion and cosmetics.
      </p>
      <router-link to="/shop" class="shop-now-btn">Shop Now</router-link>
    </div>
  </div>
</template>

<script setup>
// no JS logic needed, this is a static banner
</script>

<style scoped>
.welcome-banner {
  position: relative;
  width: 100%;
  height: 600px;
  overflow: hidden;
  border-radius: 16px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
}

.banner-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

/* overlay content */
.banner-content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: #fff;
  background: rgba(0, 0, 0, 0.25);
  padding: 40px 60px;
  border-radius: 20px;
  backdrop-filter: blur(4px);
}

.banner-title {
  font-size: 48px;
  font-weight: 800;
  margin-bottom: 10px;
}

.banner-title span {
  background: linear-gradient(90deg, #4A00E0, #8E2DE2);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.banner-subtitle {
  font-size: 18px;
  margin-bottom: 25px;
  opacity: 0.9;
}

.shop-now-btn {
  background: linear-gradient(90deg, #4A00E0, #8E2DE2);
  color: #fff;
  font-weight: 700;
  text-decoration: none;
  padding: 14px 36px;
  border-radius: 999px;
  box-shadow: 0 8px 22px rgba(142, 45, 226, 0.35);
  transition: all 0.25s ease;
}

.shop-now-btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 12px 26px rgba(142, 45, 226, 0.45);
}

@media (max-width: 768px) {
  .welcome-banner {
    height: 380px;
  }
  .banner-content {
    padding: 20px 25px;
  }
  .banner-title {
    font-size: 28px;
  }
  .banner-subtitle {
    font-size: 14px;
  }
}
</style>
