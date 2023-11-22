<script>
export default {
    data(){
        return {
            greetings: "La mia prima app con Vite!",
            mostraParagrafo: false,
        };
    },
    methods: {
        message() {
            this.mostraParagrafo = true;
        },
    },
};
</script>

<template>
    <div>
        <h2> {{ greetings }} </h2>
        <button @click="message"> cliccami! </button>
        <p v-if="mostraParagrafo"> il mio primo bottone con Vite! </p>
    </div>
    

</template>

<style>
</style>