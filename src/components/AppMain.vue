<script>
export default {
    data() {
        return {
            text: "Lorem ipsum dolor sit amet",
            imageName: 'vue.svg'
        };
    },
    methods: {
        clicked() {
            alert("Ciao da clicked");
        },
        // imageLink: function(img) {
        imageLink(img) {
            const url = new URL(`../assets/${img}`, import.meta.url);
            // console.log(url);

            const link = url.href;
            // console.log(link);

            return link;
        }
    },
};
</script>

<template>
    <main>
        <div>
            <img src="../assets/vue.svg">
            <img src="/vite.svg">
            <img :src="imageLink(imageName)">
        </div>

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
