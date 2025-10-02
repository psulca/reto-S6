<template>
  <aside class="sidebar" aria-label="Navigation menu">
    <nav>
      <ul class="nav-list">
        <li class="nav-item">
          <a href="#" class="nav-link" aria-label="Books section">Books</a>
        </li>
        <li class="nav-item">
          <a href="#" class="nav-link" aria-label="Authors section">Authors</a>
        </li>
        <li class="nav-item">
          <a href="#" class="nav-link" aria-label="Genres section">Genres</a>
        </li>
      </ul>
    </nav>
  </aside>
</template>

<script>
export default {
  name: 'SidebarComponent'
}
</script>

<style scoped>
.sidebar {
  width: 200px;
  background-color: #34495e;
  padding: 1rem 0;
  min-height: calc(100vh - 120px);
}

.nav-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.nav-item {
  margin: 0;
}

.nav-link {
  display: block;
  padding: 1rem 1.5rem;
  color: white;
  text-decoration: none;
  transition: background-color 0.3s ease;
}

.nav-link:hover {
  background-color: #2c3e50;
}

.nav-link:focus {
  outline: 2px solid #3498db;
  outline-offset: -2px;
}
</style>
