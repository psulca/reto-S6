<template>
  <div class="task-item">
    <div class="task-content">
      <h3 class="task-title">{{ title }}</h3>
      <p class="task-description">{{ description }}</p>
      <span class="task-status">{{ status }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TaskItemComponent',
  props: {
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
    status: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.task-item {
  background-color: #f8f9fa;
  border: 1px solid #dee2e6;
  border-radius: 8px;
  padding: 1rem;
  margin-bottom: 0.5rem;
  transition: box-shadow 0.3s ease;
}

.task-item:hover {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.task-content {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.task-title {
  margin: 0;
  font-size: 1.1rem;
  font-weight: 600;
  color: #2c3e50;
}

.task-description {
  margin: 0;
  color: #6c757d;
  font-size: 0.9rem;
}

.task-status {
  display: inline-block;
  padding: 0.25rem 0.5rem;
  background-color: #e9ecef;
  color: #495057;
  border-radius: 4px;
  font-size: 0.8rem;
  font-weight: 500;
  align-self: flex-start;
}
</style>
