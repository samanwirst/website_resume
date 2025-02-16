<script setup>

import MainInformation from './components/MainInformation.vue';
import SkillsInformation from './components/SkillsInformation.vue';
import FullDescription from './components/FullDescription.vue';
</script>

<template>
    <div class="lg:w-[900px] lg:p-[48px] border-[#3b4756] border mx-auto rounded-xl text-white md:p-[24px] md:w-[700px] xs:p-[16px] xs:w-[400px]">
        <MainInformation />
        <SkillsInformation />
        <FullDescription />
    </div>
</template>

<style scoped></style>
