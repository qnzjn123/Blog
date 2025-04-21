<template>
  <div class="home-container">
    <div class="hero-section">
      <div class="hero-content">
        <h1>AI와 코딩의 새로운 여정</h1>
        <p class="subtitle">디지털 세계에서 창의성과 기술의 만남</p>
      </div>
    </div>
    
    <div class="intro-section">
      <div class="intro-container">
        <div class="intro-image">
          <div class="image-placeholder">
            <div class="icon">👩‍💻</div>
          </div>
        </div>
        <div class="intro-text">
          <h2>안녕하세요, 임가을입니다</h2>
          <p>
            인공지능과 코딩의 교차점에서 새로운 가능성을 탐구하고 있습니다. 
            기술이 우리 삶을 어떻게 변화시키는지, 그리고 우리가 기술과 함께 어떻게 성장할 수 있는지에 대한 
            이야기를 이 공간에서 나누고자 합니다.
          </p>
          <p>
            인공지능이 단순한 도구를 넘어 창의적인 파트너가 되는 시대에, 
            코드와 알고리즘은 더 이상 개발자만의 영역이 아닙니다. 
            이 블로그에서는 AI와 코딩의 융합이 만들어내는 가능성에 대해 탐구하고, 
            함께 배우며 성장하는 여정을 기록합니다.
          </p>
        </div>
      </div>
    </div>
    
    <div class="topics-section">
      <div class="topics-container">
        <h2>주요 관심 분야</h2>
        <div class="topics-grid">
          <div class="topic-card">
            <div class="topic-icon">🤖</div>
            <h3>인공지능의 진화</h3>
            <p>AI 기술의 최신 동향과 발전 과정, 그리고 그것이 우리 삶에 미치는 영향에 대해 탐구합니다.</p>
          </div>
          <div class="topic-card">
            <div class="topic-icon">💻</div>
            <h3>창의적 코딩</h3>
            <p>코딩이 단순한 기술적 작업이 아닌 창의적 표현의 도구로 활용되는 방법을 공유합니다.</p>
          </div>
          <div class="topic-card">
            <div class="topic-icon">🔍</div>
            <h3>디지털 윤리</h3>
            <p>기술 발전에 따른 윤리적 질문과 우리가 나아가야 할 방향에 대해 고민합니다.</p>
          </div>
        </div>
      </div>
    </div>
    
    <div class="quote-section">
      <div class="quote-container">
        <blockquote>
          "코드는 인간의 의도를 기계에게 전달하는 언어이지만, AI의 발전과 함께 이제는 기계도 인간의 창의성을 이해하기 시작했습니다."
        </blockquote>
        <p class="quote-author">- 임가을</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style scoped>
.home-container {
  width: 100%;
}

.hero-section {
  height: 60vh;
  min-height: 400px;
  background: linear-gradient(135deg, #667eea, #764ba2);
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 0 20px;
}

.hero-content h1 {
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 1rem;
  letter-spacing: -0.5px;
}

.subtitle {
  font-size: 1.5rem;
  font-weight: 300;
  opacity: 0.9;
}

.intro-section {
  padding: 80px 20px;
  background-color: white;
}

.intro-container {
  max-width: 1000px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  gap: 40px;
}

.intro-image {
  flex: 1;
  min-width: 300px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.image-placeholder {
  width: 300px;
  height: 300px;
  border-radius: 50%;
  background: linear-gradient(45deg, #f3f4f6, #e5e7eb);
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

.icon {
  font-size: 100px;
}

.intro-text {
  flex: 2;
  min-width: 300px;
}

.intro-text h2 {
  font-size: 2.2rem;
  color: #333;
  margin-bottom: 1.5rem;
}

.intro-text p {
  font-size: 1.1rem;
  line-height: 1.8;
  color: #4b5563;
  margin-bottom: 1.5rem;
}

.topics-section {
  padding: 80px 20px;
  background-color: #f9fafb;
}

.topics-container {
  max-width: 1000px;
  margin: 0 auto;
}

.topics-container h2 {
  font-size: 2.2rem;
  color: #333;
  margin-bottom: 2.5rem;
  text-align: center;
}

.topics-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 30px;
}

.topic-card {
  background-color: white;
  border-radius: 12px;
  padding: 30px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  transition: transform 0.3s, box-shadow 0.3s;
}

.topic-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 15px rgba(0,0,0,0.1);
}

.topic-icon {
  font-size: 40px;
  margin-bottom: 20px;
}

.topic-card h3 {
  font-size: 1.3rem;
  color: #1f2937;
  margin-bottom: 15px;
}

.topic-card p {
  color: #6b7280;
  line-height: 1.6;
}

.quote-section {
  padding: 100px 20px;
  background: linear-gradient(135deg, #3b82f6, #2563eb);
  color: white;
}

.quote-container {
  max-width: 800px;
  margin: 0 auto;
  text-align: center;
}

blockquote {
  font-size: 1.8rem;
  font-style: italic;
  font-weight: 300;
  line-height: 1.6;
  margin-bottom: 20px;
}

.quote-author {
  font-size: 1.1rem;
  font-weight: 500;
}

@media (max-width: 768px) {
  .hero-content h1 {
    font-size: 2.2rem;
  }
  
  .subtitle {
    font-size: 1.2rem;
  }
  
  .intro-text h2 {
    font-size: 1.8rem;
  }
  
  .intro-text p {
    font-size: 1rem;
  }
  
  blockquote {
    font-size: 1.4rem;
  }
}
</style>
