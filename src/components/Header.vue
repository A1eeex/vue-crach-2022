<template>
  <header>
    <h1> {{ title }}</h1>
    <Button
        @btn-click="$emit('toggle-add-task')"
        :color="showAddTask? 'darkgray': 'green'"
        :title="showAddTask ? 'Close': 'Add Task' "/>
  </header>
</template>

<script>
import Button from "@/components/Button";

export default {
  name: "Header",
  props: {
    title: {
      type: String,
      default: 'hello word',
    },
    showAddTask: Boolean
  },
  components: {
    Button
  }
}
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>