<template>
    <li class="dropdown">
        <a class="nav-link text-white dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
            File
        </a>
        <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
        </ul>
    </li>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import { Dropdown } from 'bootstrap';
</script>