<template>
<p className="message">{{messageSon}}</p>
</template>

<script setup>

defineProps({
    messageSon:{ 
        type: String,
        default: "the human likes to say. that i live here rent free. but i would argue. this housing accommodation. is my payment. for a lifetime of love. and excellent company",
        }
});

</script>

