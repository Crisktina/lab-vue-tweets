<template>
    <img
      :src="imageSon"
      referrerpolicy="no-referrer"
      className="profile"
      alt="profile"
    />
</template>

<script setup>

defineProps({
    imageSon: {
      type : String,
      default: "https://i.imgur.com/b0EdHVV.jpg",}
});

</script>
