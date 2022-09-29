<template>
  <div className="tweet">
    <ProfileImage :imageSon="userFather.image" />

    <div className="body">
      <div className="top">
        <User v-bind:userSon="userFather" />
        <Timestamp :timeSon="timestampFather" />
      </div>

      <Message :messageSon="messageFather" />
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



defineProps ({
    userFather: {
      type: Object,
      },
    timestampFather: {
      type: String,
      },
    messageFather: {
      type: String,
      }});

</script>

<style scoped>
a {
  color: #42b983;
}
</style>
