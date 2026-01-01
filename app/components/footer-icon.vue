<script lang="ts" setup>
    interface Props {
        type: string,
        icon: string,
        href: string,
    }
    const {} = defineProps<Props>()
</script>

<template>
    <div class="icon-wrapper">
        <a :href="href"><Icon class="icon" :class="'icon-' + type" :name="icon"/></a>
    </div>
</template>

<style>
    .icon-wrapper {
        margin-inline: 20px;
        background: green;
        padding: 8px;
        border-radius: 8px;
    }

    .icon {
        --icon-size: 32px;
        background: lime;
        width: var(--icon-size);
        height: var(--icon-size);
    }
</style>