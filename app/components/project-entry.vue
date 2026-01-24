<script lang="ts" setup>
    interface Props {
        img: string,
        name: string,
        desc: string,
        link: string,
    }
    const {} = defineProps<Props>();
</script>

<template>
    <div class="project-entry">
        <img class="project-img" :src="img">
        <h2>{{ name }}</h2>
        <div class="project-entry-bottom">
            <p class="desc">{{ desc }}</p>
            <a :href="link">Check it out <Icon name="material-symbols:arrow-outward-rounded" /></a>
        </div>
    </div>
</template>

<style>
    :root {
        --project-img-width: 360px;
    }

    .project-entry {
        padding: 20px;
        -webkit-box-shadow: 0px 6px 22px -1px rgba(0, 0, 0, 0.349);
        box-shadow: 0px 6px 22px -1px rgba(0, 0, 0, 0.092);
        width: fit-content;
        border-radius: 20px;
        transition: 0.3s all;
        background: rgba(227, 227, 227, 0.135);
        backdrop-filter: blur(12px);
        height: fit-content;
        max-width: var(--project-img-width);
    }
    
    .project-entry:hover {
        transform: scale(1.05);
    }

    .project-img {
        transition: 0.3s all;
    }

    /*.project-entry:hover .project-img {
        transform:scale(1.05);
    }*/
    
    .project-entry>img {
        width: var(--project-img-width);
        border-radius: 12px;
        margin-bottom: 20px;
    }

    .project-entry>h2 {
        margin-bottom: 6px;
    }

    .project-entry-bottom {
        display: flex;
        flex-direction: row;
    }

    .desc {
        overflow-wrap: normal;
    }

    .project-entry-bottom>a {
        position: absolute;
        right: 20px;
        bottom: 20px;
    }

    .project-entry-bottom>a>Icon {
        position: absolute;
        top: 10px;
    }
</style>