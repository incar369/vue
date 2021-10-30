<template>
    <div class="page-4" v-if="parm">
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
    .page-4{
        position: absolute;
        display: block;
        height:875px;
        width:100%;
        background:rgb(180, 180, 180);;
    }
</style>
