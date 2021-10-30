<template>
    <div class="content">
        <a1/>
        <a2/>
        <a3/>
        <a4/>
        <a5/>
    </div>
  </template>
  
  <script>
    import a1 from './1.vue'
    import a2 from './2.vue'
    import a3 from './3.vue'
    import a4 from './4.vue'
    import a5 from './5.vue'
    export default {
        name: 'Content',
        components: {
            a1,a2,a3,a4,a5
        }
    }
  
  </script>
  
  <style scoped>
  .content{
    display:block;
    box-sizing: content-box;
    width:100%;
  }
  </style>
  