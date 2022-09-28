<template>
  <div className="tweet">
    <ProfileImage :image="user.image" />

    <div className="body">
      <div className="top">
        <User :userData="user" />
        <Timestamp :time="timestamp" />
      </div>

      <Message :message="message" />
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>

import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Timestamp from "./Timestamp.vue";
import Message from "./Message.vue";
import Actions from "./Actions.vue";

defineProps({
  name: Tweet,
  props: {
    user: {
      type: Object,
      },
    timestamp: {
      type: String,
      },
    message: {
      type: String,
      }
  }
});
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
