<template>
    <div class="page-5" v-if="parm">
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
    
    let s = screen.availHeight+' px'
    console.log(s)
</script>

<style scoped>
    .page-5{
        position: absolute;
        display: block;
        height:875px;
        width:100%;
        background:rgb(70, 70, 70);;
    }
</style>
