<template>
    <div class="page-3" v-if="parm">
    </div>
</template>

<script>
    let data = {parm:false}
    let obj = {
        data(){return data}
    }
    obj.chenge=function(a){
        data.parm = a
    }
    export default obj
</script>

<style scoped>
    .page-3{
        position: absolute;
        display: block;
        height:875px;
        width:100%;
        background:rgb(255, 175, 175);;
    }
</style>
