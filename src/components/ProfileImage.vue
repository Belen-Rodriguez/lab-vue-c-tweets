<template>
  <img :src="userImg" class="profile" alt="profile" />
</template>

<script>
export default {
  name: "ProfileImage",

  props: {
    userImg: {
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
