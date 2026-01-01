<template>
    <div class="content">
        <section class="intro">
            <h1>Hello, world!</h1>
            <p>Goodbye, world</p>
            <p>Goodbye, world</p>
            <p>Goodbye, world</p>
            <p>Goodbye, world</p>
            <a href="/blog">Go to blog</a>
            <a href="/blog">Go to blog</a>
        </section>
    </div>
</template>

<script lang="ts" setup>
    
</script>

<style>
    .content {
        height: 1900px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .intro {
        width: var(--navbar-width)
    }
</style>