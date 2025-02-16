<template>
    <section class="m-auto flex w-100 border-[#3b4756] border mt-2 rounded-xl p-4 md:flex-row xs:flex-col">
        <div>
            <img src="/photo.jpg" alt="my_photo" class="personal_photo w-[10vw] md:w-[20vw] xs:w-[70vw] xs:mx-auto">
        </div>
        <div class="personal_info ml-5">
            <h1 class="lg:text-3xl md:text-xl xs:text-2xl">Mukhammadiev Samandar</h1>
            <p class="lg:text-xl md:text-base xs:text-base">{{ age }} years old (12.09.2007)</p>
            <br>
            <div class="flex justify-between w-full">
                <div>
                    <p class="lg:text-xl md:text-sm xs:text-base">Frontend-Developer & <br>Telegram-Bots Developer</p>
                </div>
                <div class="ml-10">
                    <p class="lg:text-xl md:text-sm xs:text-base">Desired Salary: 800$</p>
                </div>
            </div>
            <br>
            <p class="lg:text-xl md:text-sm xs:text-base">Uzbekistan<br>Tashkent-Samarkand</p>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            birthDate: '2007-09-12'
        }
    },
    computed: {
        age() {
            const today = new Date();
            const birthDate = new Date(this.birthDate);
            let age = today.getFullYear() - birthDate.getFullYear();
            const monthDifference = today.getMonth() - birthDate.getMonth();

            if (monthDifference < 0 || (monthDifference === 0 && today.getDate() < birthDate.getDate())) {
                age--;
            }

            return age;
        }
    }
}
</script>