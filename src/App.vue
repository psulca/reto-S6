<template>
  <div id="app">
    <HeaderComponent />
    <div class="main-container">
      <SidebarComponent />
      <TaskListComponent />
    </div>
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/header.component.vue'
import FooterComponent from './components/footer.component.vue'
import SidebarComponent from './components/sidebar.component.vue'
import TaskListComponent from './components/task-list.component.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    FooterComponent,
    SidebarComponent,
    TaskListComponent
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

.main-container {
  display: flex;
  flex: 1;
  min-height: calc(100vh - 120px);
}
</style>
