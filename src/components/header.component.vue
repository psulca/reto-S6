<template>
  <header class="header">
    <div class="logo">
      <img src="../assets/logo.png" alt="Library Center Logo" />
    </div>
    <h1 class="title">Library Center</h1>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent'
}
</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
  padding: 1rem 2rem;
  background-color: #2c3e50;
  color: white;
  border-bottom: 2px solid #34495e;
}

.logo img {
  height: 40px;
  width: auto;
  margin-right: 1rem;
}

.title {
  margin: 0;
  font-size: 1.8rem;
  font-weight: bold;
}
</style>
