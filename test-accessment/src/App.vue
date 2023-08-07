<script setup>
import task from './components/task.vue'
</script>

<template>
  <main>
    <task />
  </main>
</template>

<style>
.todo-table {
  width: 200%;
  border-collapse: collapse;
  border: 1px solid #ccc;
  margin-top: 20px;
  margin: 0 0 0 0;
}

.todo-table th,
.todo-table td {
  border: 1px solid #ccc;
  padding: 8px;
  text-align: center;
}

.todo-table th {
  background-color: #22e279;
  font-weight: bold;
}
.edit-button,
.update-button {
  border: none;
  padding: 6px 12px;
  cursor: pointer;
  border-radius: 4px;
  font-size: 14px;
  transition: background-color 0.3s ease;
  margin: 5px;
}

.edit-button {
  background-color: #3498db;
  color: #fff;
}

.edit-button:hover {
  background-color: #2980b9;
}

.update-button {
  background-color: #27ae60;
  color: #fff;
}

.update-button:hover {
  background-color: #219653;
}
</style>