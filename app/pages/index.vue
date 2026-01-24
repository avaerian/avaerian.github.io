<template>
    <div class="page-content">
        <section id="intro">
            
            <div class="container nav-width-size">
                <div class="content">
                    <h1>Welcome to my Website</h1>
                </div>

            </div>
        </section>
        
        <section id="more">

            <div class="container nav-width-size">
                
                <div class="cool-tag">1.</div>
                <div class="precontent">
                    <!-- TODO: restructure to allow certain overflow items -->
                    <Circle size="120px", 
                        circleStyle="background:linear-gradient(135deg, #ceffad 1%,#2ad39e 100%); right: calc(var(--size) * -.4); top: calc(var(--size) * -.4);" />
                    <div class="content">
                    
                        <div class="content-left">
                            <h1>Hello, world!</h1>
                            <p>Hello, I am Avaerian, more namely Gabriel Simon, and welcome to my website!</p>
                            
                            <p>Goodbye, world</p>
                            <p>Goodbye, world</p>
                            <p>Goodbye, world</p>
                            <a href="/blog">Go to blog</a>
                        </div>

                        <div class="content-right">
                            <img src="assets/midnight_arrives_debug_photo.png" style="border-radius: 24px">
                        </div>
                    </div>
                </div>

            </div>

        </section>
        
        <section id="projects">
            <div class="container nav-width-size">
                <div class="content">
                    <span class="projects-header">
                        <h2>Explore projects</h2>
                        <a href="/projects"><p>Explore more</p><Icon class="explore-btn-icon" name="material-symbols:arrow-forward-rounded"/></a>
                    </span>
                    <div class="project-entries">
                        <ProjectEntry img="https://assets.nintendo.com/image/upload/ar_16:9,c_lpad,w_1240/b_white/f_auto/q_auto/store/software/switch/70010000000964/a28a81253e919298beab2295e39a56b7a5140ef15abdb56135655e5c221b2a3a"
                        name="Ether" desc="A skyblock project" link="https://github.com/avaerian/Ether"></ProjectEntry>
                        <ProjectEntry img="https://cms-media.roblox.com/resize=width:1280,fit:max/GnaqqRBTcCuoRELL938w"
                        name="Midnight Arrives" desc="Horror game with the goal of completing tasks to escape amidst the arachnae." link="https://www.roblox.com/games/7835879494/Midnight-Arrives-Asylum-Rework"></ProjectEntry>
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
import Circle from '~/components/circle.vue';


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

    #intro>.container {
        background-image:
            linear-gradient(rgba(53, 53, 53, 0.221) 1px, transparent 1px),
            linear-gradient(90deg, rgba(53, 53, 53, 0.221) 1px, transparent 1px);
        background-size: 1.8em 1.8em;
    }

    /*section>.container>*/.content {
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

    #more {
        flex-direction: row;
        justify-content: center;
    }
    
    #more>.container {
        position: relative;
    }

    #more>.container>.precontent {
        width: 100%;
        height: 690px;
        /* background: red; */
    }

    #more>.container>.precontent>.content {
        position: relative;
        height: 100%;
        margin-bottom: 100px;
        display: flex;
        /* background: blue; */
        flex-direction: row;
        justify-content: space-evenly;
        overflow:hidden;
        /* background: red; */
    }

    #more>.container>.precontent>.content>* {
        width: 48%;
    }
    
    #more>.container>.precontent>.content>.right-content {
        position: relative;
        max-width: 500px;
        max-height: 300px;
        width: auto;
        height: auto;
        background: url("assets/midnight_arrives_debug_photo.png");
    }

    #projects>.container {
        padding-bottom: 80px;
    }

    .projects-header {
        display: flex;
        flex-direction: row;
        align-items: center;
    }

    .projects-header>* {
        vertical-align: middle;
    }

    .projects-header>a {
        position: relative;
        display: flex;
        flex-direction: row;
        align-items: center;
        margin-left: 32px;
        padding: 8px 16px;
        border-radius: 50px;
        border: 1px solid black;
        text-decoration: none;
        color: black;
        transition: 0.3s all;
        z-index: 10;
        overflow: hidden;
    }

    .explore-btn-icon {
        position: relative;
        margin-left: 4px;
    }

    .projects-header>a:hover {
        color: white;
    }

    .projects-header>a:before {
        position: absolute;
        top: 0;
        left: 0;
        content: '';
        width: 100%;
        height: 100%;
        background: black;
        transition: 0.3s all;
        z-index: -1;
        transform: scale(0, 1);
    }

    .projects-header>a:hover:before {
        transform: scale(1,1);
    }

    .project-entries {
        position: relative;
        top: 30px;
        display: flex;
        flex-direction: row;
        justify-content: center;
        flex-wrap: wrap;
        row-gap: 24px;
        column-gap: 24px;
        width: 100%;
        height: 100%;
    }

    .project-entries>ProjectEntry {
        display: flexbox;
    }
</style>