<script>
export default {
    data() {
        return {
            text: "Lorem ipsum dolor sit amet",
        };
    },
    methods: {
        clicked() {
            alert("Ciao da clicked");
        },
    },
};
</script>

<template>
    <main>
        <p>
            {{ text }}
        </p>

        <button @click="clicked()">
            Cliccami
        </button>
    </main>
</template>

<style scoped>
p {
    color: blue;
}
</style>
