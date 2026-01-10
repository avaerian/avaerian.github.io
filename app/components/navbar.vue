<template>
    <nav>
        <div class="nav-content">
            <div class="nav-end nav-logo">
                <div class="nav-profile">
                    <img src="assets/linkedin-pfp.jpeg">
                    <a href="/"><h2>avaerian</h2></a>
                </div>
            </div>
            
            <div class="nav-center">
                <div class="nav-center-element">
                    <ul>
                        <li><a href="/">Home</a></li>
                        <li><a href="/">About</a></li>
                        <li><a href="/projects">Projects</a></li> <!-- TODO: add drop down of projects -->
                        <li><a href="/blog">Blog</a></li>
                        <li><a href="/donate">Documentation</a></li>
                    </ul>
                </div>
                <!--<div class="nav-center-element">
                    <ul>
                        <li><a href="/blog">Blog</a></li>
                        <li><a href="/donate">Donate</a></li>
                    </ul>
                </div>-->
            </div>

            <div class="nav-end nav-donate"> <!-- if used, could have a drop down of donation/tip options -->
                <ul>
                    <li class="sponsor-btn">
                        <a href="#"><Icon class="heart-icon" icon="material-symbols:favorite-outline-rounded"/><p>Sponsor</p></a>
                    </li>
                    <!-- <li><a href="#">Donate</a></li> -->
                </ul>
            </div>
        </div>
    </nav>
</template>

<script lang="ts" setup>
import { Icon } from '@iconify/vue';


</script>

<style>
    :root {
        --navbar-height: 80px;
        --navbar-width: 80%;
    }

    nav {
        position: sticky;
        width: 100%;
        height: var(--navbar-height);
        top:0;
        background: #0b0f1a;
        z-index: 10000;
        display: flex;
        justify-content: center;
    }

    .nav-profile {
        display: flex;
        flex-direction: row;
        align-items: center;
    }

    .nav-profile>a {
        color: #cfcfcf;
        text-decoration: none;
    }

    .nav-profile>* {
        margin-inline: 6px;
    }

    .nav-profile>*:first-child {
        margin-inline-start: 0;
    }

    .nav-profile>*:last-child {
        margin-inline-end: 0;
    }
    
    .nav-profile>img {
        aspect-ratio: 1;
        object-fit: contain;
        height: calc(var(--navbar-height) - 28px);
        /* height: 58px; */
        border-radius: 50%;
    }

    .nav-content {
        display: flex;
        box-sizing: border-box;
        /* flex: 0 0 1; */
        justify-content:space-between;
        /* background: gold; */
        width: var(--navbar-width);
        max-width: 1320px;
        height: 100%;
        align-items: center;
    }

    .nav-content > * {
        width: 100%;
        height: 50px;
        /* background: red; */
    }

    .nav-logo {
        /* background: yellow !important; */
        left: 0;
        justify-content: flex-end;
    }

    .nav-center {
        display: flex;
        flex-direction: row;
        width: fit-content;
        height: 50px;
        margin-inline: auto;
        /* background: red; */
    }

    .nav-center-element {
        margin-inline: 20px;
    }

    /* .nav-center-element:only-of-type {
        margin-inline: 0;
    } */

    .nav-center-element:first-child {
        margin-inline-start: 0;
    }

    .nav-center-element:last-child {
        margin-inline-end: 0;
    }

    .nav-center-element>ul {
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: row;
        padding: 0;
        list-style: none;
        background: orange;
        align-items: center; /* vertical align buttons */

    }

    .nav-center-element>ul>li {
        width: fit-content;
        height: fit-content;
        display: table;
        margin-inline: 4px;
        box-sizing: border-box;
    }

    .nav-center-element>ul>li>a {
        background-color: green;
        box-sizing: border-box;
        padding: 20px;
        text-decoration: none;
    }

    .nav-end {
        justify-content: flex-end;
    }

    .nav-donate {
        display: flex;
        justify-content: end;
    }

    .nav-donate>ul {
        display: flex;
        flex-direction: row;
        list-style: none;
        align-items: center;
        padding: 0;
    }
    
    .nav-donate>ul>li {
        height: fit-content;
    }

    .sponsor-btn>a {
        background: white;
        display: flex;
        flex-direction: row;
        align-items: center;
        padding-inline: 12px;
        padding-block: 10px;
        text-decoration: none;
    }

    .sponsor-btn>a>.heart-icon {
        width: 18px;
        height: auto;
    }

    .sponsor-btn>a>*{
        margin-inline: 3px;
    }

    .sponsor-btn>a>*:first-child {
        margin-inline-start: 0;
    }

    .sponsor-btn>a>*:last-child {
        margin-inline-end: 0;
    }
</style>