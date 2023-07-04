<template>
    <Head>
        <Title>Posts</Title>
    </Head>
    <h1>Posts Page <i class="fa-solid fa-note-sticky"></i></h1>
    <hr>
    <p>
        <NuxtLink to="/posts/1">Publicación 1</NuxtLink>
    </p>
    <p>
        <NuxtLink to="/posts/2">Publicación 2</NuxtLink>
    </p>
    <p>
        <NuxtLink to="/posts/3">Publicación 3</NuxtLink>
    </p>
</template>

<script setup>
    useHead({
        title: "Posts",
    });
</script>