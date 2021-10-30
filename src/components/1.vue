<template>
    <div class="page-1" v-if="parm">
    </div>
</template>
  
<script>
    let data = {parm:true}
    let obj = {
        data(){return data}
    }
    obj.chenge=function(a){
        data.parm = a
    }
    export default obj
</script>
  
<style scoped>
    .page-1{
        position: absolute;
        display: block;
        height:875px;
        width:100%;
         background:#4caf4f4f;                                              /*    #4caf4f[color] 4f[alpha]    */
    }
</style>
