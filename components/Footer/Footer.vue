<template>
    <footer class="mt-5 bg-dark text-white p-5">
        &copy; Nuxt - {{ date }}
    </footer>
</template>

<script setup>
    const date = new Date().getUTCFullYear();
</script>

<style scoped>
    footer {
        position: absolute;
        bottom: 0;
        width: 100%;
    }
</style>