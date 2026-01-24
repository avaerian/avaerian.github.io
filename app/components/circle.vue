<script lang="ts">
    export default {
        name: 'Circle',
        props: {
            size: {
                type: String,
            },
            circleStyle: {
                type: String,
                default: "",
            },
            zIndex: {
                type: Number,
                default: 10,
            }
        },
        computed: {
            cssVars() {
                return {
                    '--size': this.size,
                    '--circleStyle': this.circleStyle,
                    '--zIndex': this.zIndex,
                }
            }
        }
    };
</script>

<template>
    <div class="circle" :style="'--size:' + size + '; ' + circleStyle"></div>
</template>

<style scoped>
    .circle {
        position:absolute;
        border-radius:50%;
        box-shadow: inset 0px 0px 50px -12px rgba(129, 129, 129, 0.208);
        z-index: var(--zIndex);
        width: var(--size);
        height: var(--size);
    }
</style>