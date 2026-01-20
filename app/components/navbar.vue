<template>
    <header>
        <div class="nav-container">

            <div class="nav-content">
                <div class="nav-end nav-logo">
                    <div class="nav-profile">
                        <img src="assets/linkedin-pfp.jpeg">
                        <!-- review the bottom text; monospaced font,
                            maybe different colors depending on section
                            or character(s)
                        -->
                        <a href="/"><h2>[AVAERIAN.DEV]</h2></a>
                    </div>
                </div>

                <div class="nav-center">
                    <div class="nav-center-element">
                        <ul>
                            <li><a href="/">Home</a></li>
                            <li><a href="/about">About</a></li>
                            <li><a href="/projects">Projects</a></li> <!-- TODO: add drop down of projects -->
                            <li><a href="/blog">Blog</a></li>
                            <li><a href="/docs">Documentation</a></li>
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

        </div>
    </header>
</template>

<script lang="ts" setup>
import { Icon } from '@iconify/vue';


</script>

<!-- use another style block for mobile? --><style></style>

<style>
    :root {
        --navbar-height: 80px;
        --navbar-width: 80%;
        --color-blue-black: #0b0f1a;
    }

    header {
        /* position: sticky; */
        width: 100%;
        height: var(--navbar-height);
        top:0;
        /* background: var(--color-blue-black); */
        z-index: 10000;
        display: flex;
        justify-content: center;
        border-bottom: 1px solid lightgray;
    }

    /* NOTE: css for nav-width-size class will expand significantly when working
                with
    */
    .nav-container, .nav-width-size {
        width: var(--navbar-width);
        max-width: 1320px;
    }

    .nav-container {
        /* background: gold; */
        border-inline: 1px solid lightgray;
    }

    .nav-content {
        display: flex;
        box-sizing: border-box;
        /* flex: 0 0 1; */
        justify-content:space-between;
        height: 100%;
        align-items: center;

        margin-inline: 20px;
    }

    .nav-content>* {
        width: 100%;
        height: 50px;
        /* background: red; */
    }

    .nav-profile {
        display: flex;
        flex-direction: row;
        align-items: center;
    }

    .nav-profile>a {
        color: #cfcfcf;
        /* background: green; */
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
        /* background: orange; */
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
        position: relative;
        /* background-color: green; */
        color: black;
        box-sizing: border-box;
        padding: 20px;
        text-decoration: none;
        font-weight: 600;
        text-transform: uppercase;
        font-family: "Google Sans Code", monospace;
    }

    .nav-center-element>ul>li>a::before {
        position: absolute;
        bottom: 0;
        left: 0;
        background: black;
        height: 5px;
        width: 100%;
        content:'';
        transition: 0.4s all;
        transform: scale(0, 1);
        border-radius: 24px;
    }

    .nav-center-element>ul>li>a:hover::before {
        transform: scale(1, 1);
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