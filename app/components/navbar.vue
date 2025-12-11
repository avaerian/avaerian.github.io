<template>
    <nav>
        <div class="nav-content">
            <div class="nav-end nav-logo">
                <h1>avaerian</h1>
            </div>
            
            <div class="nav-center">
                <div class="nav-right">
                    <ul>
                        <li><a href="/">Home</a></li>
                        <li><a href="/projects">Projects</a></li>
                        <li><a href="/blog">Blog</a></li>
                        <li><a href="/donate">Donate</a></li>
                    </ul>
                </div>
                <div class="nav-left">
                    <ul>
                        <li><a href="/blog">Blog</a></li>
                        <li><a href="/donate">Donate</a></li>
                    </ul>
                </div>
            </div>

            <div class="nav-donate nav-end">
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
    nav {
        position: sticky;
        width: 100%;
        height: 80px;
        top:0;
        background: red;
        z-index: 10000;
        display: flex;
        justify-content: center;
    }

    .nav-content {
        display: flex;
        justify-content: space-between;
        background: gold;
        width: 80%;
        height: 100%;
        /*margin-inline: auto;*/
        align-items: center;
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
    }

    .nav-center>*>ul {
        width: 60%;
        max-width: 700px;
        display: flex;
        flex-direction: row;
        padding: 0;
        list-style: none;
        background: orange;
        align-items: center; /* vertical align buttons */

    }

    .nav-center>*>ul>li {
        width: fit-content;
        height: fit-content;
        background-color: green;
        padding: 20px;
        display: table;
    }

    .nav-end {
        background: brown;
        justify-content: flex-end;
        flex: 1;
    }

    .nav-donate {
        display: flex;
        justify-content: end;
    }

    .nav-donate>ul {
        list-style: none;
        padding: 0;
        background: white;
    }
</style>