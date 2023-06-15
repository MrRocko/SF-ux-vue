<template>
    <div class="test">Hello {{ name }}!</div>
    <ul>
        <li v-for="(notification, index) in notifications" :key="index">{{ notification }}</li>
    </ul>
</template>

<script setup>
    defineProps({
        name: String,
        notifications: Array,
    });
</script>