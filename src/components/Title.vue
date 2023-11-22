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
            console.log("click!" , this.mostraParagrafo);
            if ( this.mostraParagrafo) {
                setTimeout(() => {
                    this.mostraParagrafo = false
                    console.log("unclick!", this.mostraParagrafo);

                },5000);
            }
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