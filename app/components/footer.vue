<!-- Footer needs to be smaller -->
<template>
    <div class="footer">
        <div class="footer-content">
            <div class="footer-top">
                <FooterIcon href="https://github.com/avaerian" type="github" icon="simple-icons:github" iconstyle="background: linear-gradient(321deg,rgba(34, 193, 195, 1) 0%, rgba(253, 187, 45, 1) 100%);"/>
                <FooterIcon href="https://x.com/avaerian" type="twitter" icon="simple-icons:twitter" iconstyle="background: linear-gradient(90deg,rgba(143, 238, 255, 1) 0%, rgba(52, 98, 117, 1) 0%, rgba(95, 182, 201, 1) 0%, rgba(176, 229, 245, 1) 0%, rgba(79, 155, 255, 1) 100%);"/>
                <FooterIcon href="https://bsky.app/profile/avaerian.dev" type="bluesky" icon="simple-icons:bluesky" iconstyle="background: radial-gradient(circle,rgba(81, 184, 252, 1) 0%, rgba(120, 124, 207, 1) 0%, rgba(81, 81, 252, 1) 0%, rgba(110, 180, 255, 1) 100%);" />
                <FooterIcon href="https://youtube.com/@avaerian" type="youtube" icon="simple-icons:youtube" iconstyle="background: radial-gradient(circle,rgba(255, 104, 59, 1) 0%, rgba(252, 70, 107, 1) 100%);"/>
                <FooterIcon href="https://twitch.tv/avaerian" type="twitch" icon="simple-icons:twitch" iconstyle="background: linear-gradient(117deg,rgba(195, 110, 255, 1) 0%, rgba(116, 70, 252, 1) 100%);" />
                <FooterIcon href="https://linkedin.com/in/gabriel-n-simon" type="linkedin" icon="simple-icons:linkedin" iconstyle="background: linear-gradient(90deg,rgba(44, 201, 222, 1) 0%, rgba(102, 194, 255, 1) 50%, rgba(115, 199, 255, 1) 100%);" />
                <FooterIcon href="https://stackoverflow.com/users/14544017/avaerian" type="stackoverflow" icon="lineicons:stackoverflow" iconstyle="background: linear-gradient(90deg,rgba(255, 206, 107, 1) 0%, rgba(255, 136, 56, 1) 100%);"/>

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
                <p>Copyright © {{ new Date().getUTCFullYear().toString() }} Gabriel Simon. All rights reserved.</p>
                <p>Made with ❤️ by Gabriel Simon.</p>
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>

</script>

<style>
    .footer {
        background: rgb(17, 21, 22);
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
        color: rgb(194, 194, 194);
    }

    .footer-bottom>*:first-child {
        margin-block-start: 0;
    }

    .footer-bottom>*:last-child {
        margin-block-end: 0;
    }
</style>