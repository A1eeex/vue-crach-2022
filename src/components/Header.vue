<template>
  <header>
    <h1> {{ title }}</h1>
    <Button color="green" title="Add +"/>
    <Button color="red" title="update"/>
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