<template>
    <div class="container">
        <input v-model="name">
        <input v-model="passwd">
        <button v-on:click="greet">Greet</button>
    </div>
</template>

<script>
export default {
    data () {
        return {
            name: "123",
            passwd: "123"
        }
    },
    methods: {
        greet: async function (event) {
            alert('Hello ' + this.name + ' ' + this.passwd);
            this.name = "";
            this.passwd = ""
        }
    }
}
</script>

