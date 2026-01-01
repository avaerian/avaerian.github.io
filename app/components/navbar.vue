<template>
    <nav>
        <div class="nav-content">
            <div class="nav-end nav-logo">
                <h1>avaerian</h1>
            </div>
            
            <div class="nav-center">
                <div class="nav-center-element">
                    <ul>
                        <li><a href="/">Home</a></li>
                        <li><a href="/projects">Projects</a></li>
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

            <div class="nav-end nav-donate">
                <ul>
                    <li><a href="#">Sponsor</a></li>
                    <li><a href="#">Donate</a></li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script lang="ts" setup>

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
        /* background: red; */
        z-index: 10000;
        display: flex;
        justify-content: center;
    }

    .nav-content {
        display: flex;
        box-sizing: border-box;
        /* flex: 0 0 1; */
        justify-content:space-between;
        background: gold;
        width: var(--navbar-width);
        max-width: 1400px;
        height: 100%;
        align-items: center;
    }

    .nav-content > * {
        width: 100%;
    }

    .nav-logo {
        background: yellow !important;
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
    }

    .nav-end {
        background: brown;
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
        padding: 0;
        background: white;
    }

    .nav-donate>ul>li>a {
        text-decoration: n;
    }
</style>