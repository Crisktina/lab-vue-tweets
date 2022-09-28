<template>

 <span className="user">
     <span className="name">{{user.name}}</span>
     <span className="handle">{{user.handle}}</span>
 </span>

</template>


<script setup>

const props = defineProps({
    userData: Object,
});

</script>

