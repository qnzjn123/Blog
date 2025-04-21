<template>
  <div class="about">
    <h1>소개</h1>
    <p>이 웹사이트는 Vue3를 사용하여 만든 기본 사이트입니다.</p>
    <p>Vue3의 다양한 기능을 탐색하고 학습하는 데 사용할 수 있습니다.</p>
    
    <div class="team-section">
      <h2>우리 팀</h2>
      <div class="team">
        <div class="team-member" v-for="member in team" :key="member.name">
          <div class="avatar">{{ member.initials }}</div>
          <h3>{{ member.name }}</h3>
          <p>{{ member.role }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      team: [
        { name: '홍길동', role: '프론트엔드 개발자', initials: 'HGD' },
        { name: '김철수', role: '디자이너', initials: 'KCS' },
        { name: '이영희', role: '프로젝트 매니저', initials: 'LYH' }
      ]
    }
  }
}
</script>

<style scoped>
.about {
  padding: 20px 0;
}

.team-section {
  margin-top: 40px;
}

.team {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  margin-top: 20px;
}

.team-member {
  flex: 1;
  min-width: 200px;
  padding: 20px;
  background-color: #f9f9f9;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  text-align: center;
}

.avatar {
  width: 60px;
  height: 60px;
  background-color: #42b983;
  color: white;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto 15px;
  font-size: 18px;
  font-weight: bold;
}
</style>
