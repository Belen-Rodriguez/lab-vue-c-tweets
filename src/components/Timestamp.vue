<template>
  <span class="timestamp">{{ timeStamp }}</span>
</template>

<script>
export default {
  name: "Timestamp",

  props: {
    timeStamp: {
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
