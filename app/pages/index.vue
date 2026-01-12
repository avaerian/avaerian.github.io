<template>
    <div class="page-content">
        <section class="intro">
            
            <div class="container nav-width-size">
                <div class="content">
                    <h1>Hello, world!</h1>
                    <p>Goodbye, world</p>
                    <p>Goodbye, world</p>
                    <p>Goodbye, world</p>
                    <p>Goodbye, world</p>
                    <a href="/blog">Go to blog</a>
                    <a href="/blog">Go to blog</a>
                </div>

            </div>
        </section>
        
        <section class="more">
            
            <div class="container nav-width-size">
                <div class="cool-tag">1.</div>
                <div class="content">
                    <h1>Hello, world!</h1>
                    <p>Goodbye, world</p>
                    <p>Goodbye, world</p>
                    <p>Goodbye, world</p>
                    <p>Goodbye, world</p>
                    <a href="/blog">Go to blog</a>
                    <a href="/blog">Go to blog</a>
                </div>

            </div>

        </section>
        
        <section class="more2">
            <div class="container nav-width-size">
                <div class="content">
                    <h2>Explore projects</h2>
                </div>
            </div>
        </section>
    </div>
</template>

<script lang="ts" setup>

</script>

<style>
/* TODO: create standard style (w/ classes) for default center area/container */

/* For current classes/styling setup,  */

    /* :root { FOR VARIABLES LIKE BORDER (move to different file)

    } */

    .page-content {
        /* display: flex;
        flex-direction: column;
        align-items: center; */
        background-size: 40px 40px;
    }

    section {
        width: 100%;
        border-bottom: 1px solid lightgray;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    
    .container {
        border-inline: 1px solid lightgray;
    }

    .intro>.container {
        background-image:
            linear-gradient(rgba(0, 119, 255, 0.221) 1px, transparent 1px),
            linear-gradient(90deg, rgba(0, 119, 255, 0.162) 1px, transparent 1px);
        background-size: 1.8em 1.8em;
    }

    /* .intro>.container>.content {
        margin: 28px;
    } */

    section>.container>.content {
        margin: 28px;
    }

    .cool-tag {
        position: absolute;
        display: flex;
        align-items: center;
        justify-content: center;
        width: 50px;
        height: 50px;
        top: 0;
        left: 0;
        text-align: center;
        border-left: 1px solid lightgray;
        border-bottom: 1px solid lightgray;
        transform:translate(-100%);
    }

    .more {
        flex-direction: row;
        justify-content: center;
    }
    
    .more>.container {
        position: relative;
    }

    .more>.container>.content {
        height: 690px;
        /* background: red; */
    }

    .more2>.container>.content {
        height: 690px;
        /* background: blue; */
    }
</style>