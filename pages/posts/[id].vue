<template>
    <Head>
        <Title>
            Post {{ id }}
        </Title>
    </Head>
    <h2>Bienvenido al Post #{{ id }}</h2>
    <hr>
    <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora ab doloremque veritatis est rerum qui iste officia sapiente eveniet deleniti voluptate, quas aut vero dolorem molestias rem beatae provident reprehenderit?
    </div>
    <div class="d-flex justify-content-start pt-5">
        <span class="text-muted">Autor: </span> <u class="fw-semibold"> Joaquin Centurion</u>
    </div>
</template>

<script setup>
    const { id } = useRoute().params;
    if(!/^[0-9]+$/.test(id)){
        throw createError({ statusCode: "400", statusMessage: "Param type is invalid" })
    }
</script>