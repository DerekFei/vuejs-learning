<template>
    <div>
        <h3>New Quote </h3>
        <button @click="counter++"> Increase!</button>
        <div>{{counter}}</div>
    </div>
</template>
<script>
    export default {
        data: function(){
            return {
                counter: 0
            };
        },
        destroyed(){
            console.log('Destroyed!');
        },
        deactivated(){
            console.log('Deactivated');
        },
        activated(){
            console.log('activated');
        }
    }
</script>
<style scoped>

</style>