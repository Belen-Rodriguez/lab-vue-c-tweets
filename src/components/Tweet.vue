<template>
  <div class="tweet">
    <ProfileImage :userImg="eachTweet.user.image" />

    <div class="body">
      <div class="top">
        <User :userData="eachTweet.user" />
        <Timestamp :timeStamp="eachTweet.timestamp" />
      </div>
      <Message :userMessage="eachTweet.message" />
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Timestamp from "./Timestamp.vue";
import Message from "./Message.vue";
import Actions from "./Actions.vue";

export default {
  name: "Tweet",
  props: {
    eachTweet: {
      type: Object,
    },
  },

  components: {
    ProfileImage,
    User,
    Timestamp,
    Message,
    Actions,
  },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
