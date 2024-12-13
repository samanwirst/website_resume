<template>
    <section class="m-auto">
        <div>
            <img src="/photo.jpg" alt="my_photo" class="personal_photo w-40">
        </div>
        <div class="personal_info">
            <h1>Мухаммадиев Самандар</h1>
            <p>{{ age }} лет (12.09.2007)</p>
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

<style scoped>
/* .container {
    display: block;
}

section {
    display: flex;
    flex-direction: row;
    width: 100%;
    height: fit-content;
    justify-content: center;
}

.personal_photo {
    width: 200px;
    height: auto;
}
.personal_info {
    margin-left: 20px;
} */
</style>