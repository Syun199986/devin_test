<template>
  <div class="container">
    <h1>{{ inputText || 'ここに入力したテキストが表示されます' }}</h1>
    <div class="input-container">
      <input 
        type="text" 
        v-model="inputText" 
        placeholder="ここにテキストを入力してください"
        class="text-input"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      inputText: ''
    }
  }
}
</script>

<style>
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem;
  text-align: center;
  font-family: Arial, sans-serif;
}

h1 {
  margin-bottom: 2rem;
  color: #333;
  min-height: 2rem;
}

.input-container {
  margin-top: 2rem;
}

.text-input {
  width: 100%;
  padding: 0.75rem;
  font-size: 1rem;
  border: 1px solid #ccc;
  border-radius: 4px;
}
</style>
