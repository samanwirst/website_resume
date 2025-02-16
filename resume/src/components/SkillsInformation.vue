<template>
    <section class="m-auto flex justify-between w-100 border-solid border-[#3b4756] border mt-2 rounded-xl p-4 md:flex-row xs:flex-col">
        <div class="xs:my-[10px]">
            <h1 class="lg:text-3xl mb-2 xs:text-lg">Hard Skills:</h1>
            <ul>
                <li class="lg:text-xl font-bold xs:text-sm" v-for="skill in hardSkillsList">— <span :style="{ color: skill.color }">{{
                        skill.name }} ({{ skill.version }})</span></li>
            </ul>
        </div>
        <div class="xs:my-[10px]">
            <h1 class="lg:text-3xl mb-2 xs:text-lg">Soft Skills:</h1>
            <ul>
                <li class="lg:text-xl font-bold xs:text-sm" v-for="skill in softSkillsList">— <span :style="{ color: skill.color }">{{
                        skill.name }}</span></li>
            </ul>
        </div>
        <div class="xs:my-[10px]">
            <h1 class="lg:text-3xl mb-2 xs:text-lg">Languages:</h1>
            <ul>
                <li class="lg:text-xl font-bold xs:text-sm" v-for="skill in languagesList">— <span :style="{ color: skill.color }">{{
                        skill.name }}</span></li>
            </ul>
        </div>
    </section>
</template>
<script>
export default {
    data() {
        return {
            hardSkillsList: [
                {
                    name: "Vue.js",
                    version: "Vue3",
                    color: "#42b883"
                },
                {
                    name: "Next.js",
                    version: "latest",
                    color: "#FFFFFF"
                },
                {
                    name: "Nuxt.js",
                    version: "Nuxt3",
                    color: "#00DC82"
                },
                {
                    name: "Aiogram",
                    version: "2.x/3.x",
                    color: "#2CA5E0FF"
                },
                {
                    name: "Docker",
                    version: "latest",
                    color: "#2496EDFF"
                },
                {
                    name: "Git",
                    version: "latest",
                    color: "#F14C28"
                },
                {
                    name: "API Integration",
                    version: "latest",
                    color: "#66ccff"
                },
                {
                    name: "Linux",
                    version: "Ubuntu, Arch, Debian",
                    color: "#FCC624FF"
                }
            ],
            softSkillsList: [
                {
                    name: "Adaptability",
                    color: "#4CAF50"
                },
                {
                    name: "Problem Solving",
                    color: "#2196F3"
                },
                {
                    name: "Leadership Skills",
                    color: "#D32F2FFF"

                }
            ],
            languagesList: [
                {
                    name: "Russian (native)",
                    color: "#b22234"
                },
                {
                    name: "English C1 (IELTS 7.0)",
                    color: "#003da5"
                }
            ]
        }
    }
}
</script>