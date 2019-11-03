<template>
    <div class="component">
        <h3>You may view the User Details here</h3>
        <p>Many Details</p>
        <p>UserName:{{ switchName() }}</p>
        <button @click="resetName()">Reset Name</button>
        <button @click="reserFn()">Reset Name </button>
        <button></button>
    </div>
</template>

<script>
    export default {
        data: function () {
            return{

            }
        },
        methods:{
            switchName(){

            },
            resetName(){

            },
            resetFn(){

            }
        }
    }
</script>

<style scoped>
    div {
        background-color: lightcoral;
    }
</style>
