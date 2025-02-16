<template>
    <section class="border-[#3b4756] border mt-2 rounded-xl p-4">
        <h1 class="lg:text-3xl mb-2 xs:text-lg">Portfolio:</h1>
        <div v-for="project in projectList">
            <h1 class="lg:text-xl md:my-0 xs:text-sm xs:my-[12px]">— <a :href="project.link" class="underline hover:no-underline">{{ project.name }}</a>
            </h1>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            projectList: [
                {
                    name: "EIT, Admin Panel",
                    link: "https://youtu.be/tkyBZC-ESj4",
                }, 
                {
                    name: "Game of Life, Tutorial Article",
                    link: "https://habr.com/ru/articles/689918/",
                },
                {
                    name: "HTML HitBoxes, Tutorial Article",
                    link: "https://habr.com/ru/articles/690370/",
                },
                {
                    name: "Sierpiński Triangle, Tutorial Article",
                    link: "https://habr.com/ru/articles/740658/",
                },
                {
                    name: "TrueMafia Web-App",
                    link: "https://youtu.be/Z1Pnsd1wAuw",
                },
                {
                    name: "TrueMafia Web-App, page building example",
                    link: "https://youtu.be/3wgP5QxvLE8",
                },
                {
                    name: "TrueMafia Web-App, theme colors sync",
                    link: "https://youtu.be/1IcLluXkte4",
                },
                {
                    name: "Userbot Translator",
                    link: "https://github.com/samanwirst/tg_userbot_translator",
                },
                {
                    name: "Yandex Music Bot",
                    link: "https://github.com/samanwirst/yandex_music_telegram_bot",
                },
                {
                    name: "Virtual Anonim Room",
                    link: "https://github.com/samanwirst/telegram_anonim_room_bot",
                },
                {
                    name: "Userbot + Fusion Brain, AI Image Generation",
                    link: "https://github.com/samanwirst/tg_userbot_fusion_ai",
                },
                {
                    name: "Telegram automated channel posting via ChatGPT, Bot",
                    link: "https://github.com/samanwirst/tg_userbot_fusion_ai",
                },
                {
                    name: "This page",
                    link: "https://github.com/samanwirst/website_resume/tree/main/resume",
                },
            ]
        }
    }
}
</script>