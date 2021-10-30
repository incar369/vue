<template>
    <div class="page-2" v-if="parm">
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
    .page-2{
        position: absolute;
        display: block;
        height:875px;
        width:100%;
        background:rgb(175, 216, 255);
    }
</style>
