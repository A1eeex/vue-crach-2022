<template>
  <button @click="onClick()" :style="{background:color}" class="btn">{{ title }}</button>
</template>

<script>
export default {
  name: "Button",
  props: {
    title: {
      type: String,
      default: 'button',
    },
    color: String
  },
  methods: {
    onClick(){
      console.log('yo')
    }
  }
}

</script>

<style scoped>

</style>