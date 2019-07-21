<template>
    <div id="Counter">
        <table>
            <ul id="counterNum">{{counter}}</ul>
            <ul>
                <button @click="addCounter">点我+</button>
                <button @click="reduceCounter">点我-</button>
            </ul>
        </table>
    </div>
</template>

<script>
    export default {
        
        name: "Counter",
        data:function(){
            return{
                counter:0
            }
        },
        methods:{
            addCounter:function () {
                this.counter ++;
                
            },
            reduceCounter:function () {
                this.counter --;
                
            }
        },
    }
</script>

<style scoped>
#Counter {
    /*align-content: center;*/
    /*width: 200px;*/
    margin: auto;
}
</style>