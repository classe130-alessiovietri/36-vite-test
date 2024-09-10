<script>
/* 
  1) Importazione del componente
  2) Dichiarazione del componente
  3) Utilizzo del componente
*/
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";

export default {
    data() {
        return {
            message: "Ciao",
        };
    },
    components: {
        AppHeader,
        AppMain,
    }
};
</script>

<template>
    <div>
        <AppHeader />
        <AppMain />
        <AppMain />
        <AppMain />
        <AppMain />
        <AppMain />
        <AppMain />
        <AppMain />
        <AppMain />

        <p>
            LOREM IPSUM DOLOR
        </p>
    </div>
</template>

<style scoped>
p {
    color: red;
}
</style>
