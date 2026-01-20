<template>
    <div class="page-content">
        <section class="intro">
            
            <div class="container nav-width-size">
                <div class="content">
                    <h1>Welcome to my Website</h1>
                </div>

            </div>
        </section>
        
        <section class="more">

            <div class="container nav-width-size">
                <div class="circle c1" style="left: -170px; top: 100px;"></div>
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
                    <div class="projects">
                        <ProjectEntry img="https://assets.nintendo.com/image/upload/ar_16:9,c_lpad,w_1240/b_white/f_auto/q_auto/store/software/switch/70010000000964/a28a81253e919298beab2295e39a56b7a5140ef15abdb56135655e5c221b2a3a"
                        name="Ether" desc="A skyblock project" link="https://github.com/avaerian/Ether"></ProjectEntry>
                        <ProjectEntry img="https://assets.nintendo.com/image/upload/ar_16:9,c_lpad,w_1240/b_white/f_auto/q_auto/store/software/switch/70010000000964/a28a81253e919298beab2295e39a56b7a5140ef15abdb56135655e5c221b2a3a"
                        name="Hello, world!" desc="Goodbye, world!" link="https://github.com/avaerian/Ether"></ProjectEntry>
                        <ProjectEntry img="https://assets.nintendo.com/image/upload/ar_16:9,c_lpad,w_1240/b_white/f_auto/q_auto/store/software/switch/70010000000964/a28a81253e919298beab2295e39a56b7a5140ef15abdb56135655e5c221b2a3a"
                        name="Hello, world!" desc="Goodbye, world!" link="https://github.com/avaerian/Ether"></ProjectEntry>
                        <ProjectEntry img="https://assets.nintendo.com/image/upload/ar_16:9,c_lpad,w_1240/b_white/f_auto/q_auto/store/software/switch/70010000000964/a28a81253e919298beab2295e39a56b7a5140ef15abdb56135655e5c221b2a3a"
                        name="Hello, world!" desc="Goodbye, world!" link="https://github.com/avaerian/Ether"></ProjectEntry>
                    </div>
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

    .circle {
        position:absolute;
        background:linear-gradient(135deg, #ceffad 1%,#2ad39e 100%);;
        border-radius:50%;
        box-shadow: inset 0px 0px 50px -12px rgba(129, 129, 129, 0.208);
        z-index:3;
    }

    .c1 {
        width: 120px;
        height: 120px;
    }

    .projects {
        position: relative;
        top: 30px;
        display: flex;
        flex-direction: row;
        row-gap: 24px;
        column-gap: 24px;
        /* background: red; */
        width: 100%;
        height: 100%;
    }
</style>