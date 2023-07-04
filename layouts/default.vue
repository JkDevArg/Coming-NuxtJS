<template>
    <div>
        <Navbar />
        <main class="container p-3 my-5 border rounded shadow">
            <slot></slot>
        </main>
        <Footer />
    </div>
</template>

<script setup>

    useHead({
        titleTemplate: "%s - NuxtJS",
        bodyAttrs: [{
            class: "text-center",
        }],
        link: [
            {
                rel: "stylesheet",
                href: "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css",
                integrity: "sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM",
                crossorigin: "anonymous",
            },
            {
                rel: "stylesheet",
                href: "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css",
            },
        ],
        script: [
            {
                src: "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js",
            },
            {
                src: "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/js/all.min.js",
            }
        ],
    });
</script>