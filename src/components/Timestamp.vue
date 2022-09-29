<template>

<span className="timestamp">{{timeSon}}</span>
 
</template>

<script setup>

defineProps({
    timeSon: { 
        type: String,
        default: () => {
            let date = new Date();
            return date.toISOString().split("T")[0];
            },
}});


</script>


