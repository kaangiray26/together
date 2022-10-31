<template>
    <div>
        <NavBar />
        {{ title }}
    </div>
    <gCalendar />
</template>

<script setup>
import { ref, onMounted } from 'vue';
import NavBar from '/components/NavBar.vue';
import gCalendar from '/components/gCalendar.vue';

const title = ref(null);

onMounted(() => {
    title.value = 'Hello world!';
});
</script>