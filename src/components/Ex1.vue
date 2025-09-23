<script>
    export default { 
        data () {
            return {
                message: "Choose your favourite fruit: ",
                fruits: ['apple', 'orange', 'banana']
            }
        },
        methods: {

        }  
    }
</script>

<template>
    <div id="app">
        {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit">
        <h3>Using Array</h3>
        <span v-for="fruit in fruits" :key="fruits">
            {{fruit}} <input type="radio" name="fruit">
        </span>
    </div>
</template>

<style scoped>
</style>
