<template>
    <div class="footer">
        <div class="footer-content">
            <div class="footer-top">
                <FooterIcon href="https://github.com/avaerian" type="github" icon="simple-icons:github" />
                <FooterIcon href="https://x.com/avaerian" type="github" icon="simple-icons:twitter" />
                <FooterIcon href="https://bsky.app/profile/avaerian.bsky.social" type="github" icon="simple-icons:bluesky" />
                <FooterIcon href="https://youtube.com/@avaerian" type="youtube" icon="simple-icons:youtube" />
                <FooterIcon href="https://twitch.tv/avaerian" type="twitch" icon="simple-icons:twitch" />
                <FooterIcon href="https://linkedin.com/in/gabriel-n-simon" type="linkedin" icon="simple-icons:linkedin" />
                <FooterIcon href="https://stackoverflow.com/users/14544017/avaerian" type="stackoverflow" icon="lineicons:stackoverflow" />

                <!--<a><Icon class="icon icon-paypal" name="cib:paypal"/></a> alt: cib:cc-paypal -->
                <!-- blog posts icons
                <a><Icon class="icon icon-instagram" name="streamline-logos:messages-logo-solid"/></a>
                <a><Icon class="icon icon-instagram" name="jam:messages"/></a>
                <a><Icon class="icon icon-instagram" name="charm:messages"/></a>
                <a><Icon class="icon icon-instagram" name="pajamas:messages"/></a>
                -->
            </div>
            <div class="footer-bottom">
                <!-- TODO: switch this to be inserted using TS with Date/Time API -->
                <p>Copyright © 2025 Gabriel Simon. All rights reserved.</p>
                <p>Made with ❤️ by Gabriel Simon.</p>
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>


</script>

<style>
    .footer {
        background: lightblue;
        height: 240px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .footer-content {
        /* background: red; */
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .footer-content > * {
        margin-block: 24px;
    }

    .footer-top {
        /* background: lightgrey; */
        width: fit-content;
        display: flex;
        justify-content: center;
    }

    .footer-bottom {
        /* background: darkgray; */
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .footer-bottom>* {
        margin-block: 4px;
    }

    .footer-bottom>*:first-child {
        margin-block-start: 0;
    }

    .footer-bottom>*:last-child {
        margin-block-end: 0;
    }
</style>