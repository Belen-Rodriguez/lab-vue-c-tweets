<template>
  <p class="message">{{ userMessage }}</p>
</template>

<script>
export default {
  name: "Timestamp",

  props: {
    userMessage: {
      type: String,
    },
  },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
