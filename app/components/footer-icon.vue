<script lang="ts" setup>
    interface Props {
        type: string,
        icon: string,
        href: string,
        iconstyle?: string,
    }
    const {} = defineProps<Props>()
</script>

<template>
		<!-- reconsider icon-wrapper -->
    <div class="icon-wrapper">
        <a :href="href"><Icon class="icon" :class="'icon-' + type" :name="icon" :style="iconstyle"/></a>
    </div>
</template>

<style>
    .icon-wrapper {
        position: relative;
        margin-inline: 20px;
        padding: 8px;
        /* background: rgba(182, 182, 182, 0.487); */
        border-radius: 8px;
    }

		@media (max-width: 500px) {
        .icon-wrapper {
						padding: 4px;
            margin-inline: 4%;
        }
    }

    .icon-wrapper::before {
        position: relative;
        content: '';
        backdrop-filter: blur(8px);
        transform: scale(0);
        transition: 0.4s all;
    }

    .icon-wrapper:hover::before {
        transform: scale(1);
    }

    .icon {
        --icon-size: 32px;
        background: lime;
        width: var(--icon-size);
        height: var(--icon-size);
    }
</style>