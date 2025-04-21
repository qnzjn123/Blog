<template>
  <div class="contact">
    <h1>연락처</h1>
    <p>문의사항이 있으시면 아래 양식을 통해 연락해 주세요.</p>
    
    <form @submit.prevent="submitForm" class="contact-form">
      <div class="form-group">
        <label for="name">이름</label>
        <input type="text" id="name" v-model="form.name" required>
      </div>
      
      <div class="form-group">
        <label for="email">이메일</label>
        <input type="email" id="email" v-model="form.email" required>
      </div>
      
      <div class="form-group">
        <label for="message">메시지</label>
        <textarea id="message" v-model="form.message" rows="5" required></textarea>
      </div>
      
      <button type="submit">보내기</button>
    </form>
    
    <div v-if="submitted" class="success-message">
      메시지가 성공적으로 전송되었습니다!
    </div>
  </div>
</template>

<script>
export default {
  name: 'Contact',
  data() {
    return {
      form: {
        name: '',
        email: '',
        message: ''
      },
      submitted: false
    }
  },
  methods: {
    submitForm() {
      // 여기에서 실제 폼 제출 로직을 구현할 수 있습니다
      console.log('Form submitted:', this.form);
      this.submitted = true;
      this.form = { name: '', email: '', message: '' };
      
      // 3초 후에 성공 메시지 숨기기
      setTimeout(() => {
        this.submitted = false;
      }, 3000);
    }
  }
}
</script>

<style scoped>
.contact {
  padding: 20px 0;
}

.contact-form {
  max-width: 600px;
  margin: 30px 0;
}

.form-group {
  margin-bottom: 20px;
}

.form-group label {
  display: block;
  margin-bottom: 5px;
  font-weight: bold;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #ddd;
  border-radius: 4px;
  font-size: 16px;
}

button {
  background-color: #42b983;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  font-size: 16px;
  cursor: pointer;
}

button:hover {
  background-color: #3aa876;
}

.success-message {
  margin-top: 20px;
  padding: 10px;
  background-color: #d4edda;
  color: #155724;
  border-radius: 4px;
}
</style>
