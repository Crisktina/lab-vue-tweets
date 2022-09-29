<template>
    <img
      :src="image"
      referrerpolicy="no-referrer"
      className="profile"
      alt="profile"
    />
</template>

<script setup>

const props = defineProps({
    image: String,
});

</script>
