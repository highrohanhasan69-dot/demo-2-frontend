<template>
  <section class="welcome-banner">
    <div class="content">
      <h1 class="title">Welcome to <span>URBILUX</span></h1>
      <p class="subtitle">
        Discover elegant and affordable fashion & cosmetics, tailored for your sophisticated taste.
      </p>
      <router-link to="/shop" class="shop-btn">Shop Now</router-link>
    </div>
  </section>
</template>

<script setup>
// Static component — no JS needed
</script>

<style scoped>
/* 🟣 Full Banner Section */
.welcome-banner {
  width: 100%;
  height: 480px;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: linear-gradient(180deg, #4A00E0 0%, #8E2DE2 100%);
  color: #fff;
  border-radius: 0 0 40px 40px;
  position: relative;
  overflow: hidden;
}

/* 🟣 Content Center */
.content {
  max-width: 750px;
  padding: 0 20px;
}

/* 🟣 Title */
.title {
  font-size: 44px;
  font-weight: 800;
  margin-bottom: 10px;
  letter-spacing: 0.3px;
}

.title span {
  background: linear-gradient(90deg, #ffffff, #dcd0ff);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

/* 🟣 Subtitle */
.subtitle {
  font-size: 18px;
  opacity: 0.92;
  margin-bottom: 30px;
  line-height: 1.6;
}

/* 🟣 Shop Now Button */
.shop-btn {
  background: #fff;
  color: #6a11cb;
  font-weight: 700;
  text-decoration: none;
  padding: 12px 32px;
  border-radius: 999px;
  font-size: 16px;
  box-shadow: 0 8px 25px rgba(255,255,255,0.25);
  transition: all 0.25s ease;
}

.shop-btn:hover {
  background: #f4f4f4;
  transform: translateY(-3px);
}

/* 🟣 Responsive */
@media (max-width: 768px) {
  .welcome-banner {
    height: 360px;
    border-radius: 0 0 20px 20px;
  }
  .title {
    font-size: 26px;
  }
  .subtitle {
    font-size: 14px;
    margin-bottom: 20px;
  }
  .shop-btn {
    font-size: 14px;
    padding: 10px 26px;
  }
}
</style>
