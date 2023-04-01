<template>
  <span class="user">
    <span class="name">{{ userData.name }}</span>
    <span class="handle">{{ userData.handle }}</span>
  </span>
</template>

<script>
export default {
  name: "User",

  props: {
    userData: {
      type: Object,
      name: {
        type: String,
      },
      handle: {
        type: String,
      },
    },
  },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
