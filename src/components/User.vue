<template>

 <span className="user">
     <span className="name">{{userSon.name}}</span>
     <span className="handle">{{userSon.handle}}</span>
 </span>

</template>


<script setup>

defineProps({
    userSon: {
        type: Object,
        default: () => ({
         name: "Firulais puppy",
         handle: "@Firulais",
            }),
    }
});

</script>

