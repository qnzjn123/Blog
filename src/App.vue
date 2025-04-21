<template>
  <div class="app-container">
    <nav class="menu-bar">
      <div class="menu-content">
        <div class="logo">임가을 블로그</div>
        <div class="center-menu">
          <div class="home-link">홈</div>
        </div>
        <div class="placeholder"></div>
      </div>
    </nav>
    
    <main>
      <Home />
    </main>
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style>
.app-container {
  width: 100%;
  min-height: 100vh;
}

.menu-bar {
  width: 100%;
  height: 60px;
  background-color: #ffffff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  position: fixed;
  top: 0;
  left: 0;
  z-index: 100;
}

.menu-content {
  max-width: 1200px;
  height: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;
}

.logo {
  font-size: 22px;
  font-weight: 700;
  color: #3b82f6;
  cursor: pointer;
  letter-spacing: -0.5px;
  flex: 1;
}

.center-menu {
  flex: 1;
  display: flex;
  justify-content: center;
}

.placeholder {
  flex: 1;
}

.home-link {
  font-size: 18px;
  font-weight: 500;
  cursor: pointer;
  padding: 10px 20px;
  border-radius: 4px;
  transition: background-color 0.2s;
}

.home-link:hover {
  background-color: #f5f5f5;
}

main {
  padding-top: 80px;
}
</style>
