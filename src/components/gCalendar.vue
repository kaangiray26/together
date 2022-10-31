<template></template>
<script setup>
import { ref, onMounted } from 'vue';

async function authorize() {
    fetch('https://accounts.google.com/o/oauth2/v2/auth?' + new URLSearchParams({
        client_id: '1090438036378-mrarf07gv714p02v6g8b128o4q7f9ec0.apps.googleusercontent.com',
        redirect_uri: 'http://localhost:8000/oauth',
        response_type: 'token',
        scope: 'https://www.googleapis.com/auth/calendar.events.readonly',
    }), {
        method: 'GET',
        headers: {
            'Content-Type': 'application/json'
        },
    }).then(response => {
        console.log(response);
    });
}

onMounted(() => {
    authorize();
});
</script>