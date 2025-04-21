<template>
  <div class="home">
    <h1>Vue3 기본 사이트에 오신 것을 환영합니다</h1>
    <p>이 사이트는 Vue3로 만든 기본 사이트입니다.</p>
    
    <div class="feature-section">
      <h2>주요 기능</h2>
      <div class="features">
        <div class="feature-card" v-for="feature in features" :key="feature.title">
          <h3>{{ feature.title }}</h3>
          <p>{{ feature.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      features: [
        { 
          title: 'Vue3 Composition API', 
          description: 'Vue3의 새로운 Composition API를 활용한 더 나은 코드 구성' 
        },
        { 
          title: '반응형 디자인', 
          description: '모든 화면 크기에 맞게 최적화된 디자인' 
        },
        { 
          title: 'Vue Router', 
          description: 'SPA를 위한 강력한 라우팅 기능' 
        }
      ]
    }
  }
}
</script>

<style scoped>
.home {
  padding: 20px 0;
}

.feature-section {
  margin-top: 40px;
}

.features {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 20px;
  margin-top: 20px;
}

.feature-card {
  padding: 20px;
  background-color: #f9f9f9;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}
</style>
