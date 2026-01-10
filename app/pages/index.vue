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
        <section class="more">

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
        background-size: 40px 40px;
        background-color: lightgray;
        background-image: 
            linear-gradient(rgba(0, 119, 255, 0.221) 1px, transparent 1px), 
            linear-gradient(90deg, rgba(0, 119, 255, 0.162) 1px, transparent 1px);
    }

    .intro {
        width: var(--navbar-width)
    }
</style>