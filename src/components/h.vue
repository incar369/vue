<template>
  <div class="header">
    <button class='b1' id='n1' v-on:click="visablePage">1</button>
    <button class='b2' id='n2' v-on:click="visablePage">2</button>
    <button class='b3' id='n3' v-on:click="visablePage">3</button>
    <button class='b4' id='n4' v-on:click="visablePage">4</button>
    <button class='b5' id='n5' v-on:click="visablePage">5</button>
  </div>
</template>

<script>
import a1 from './1.vue'
import a2 from './2.vue'
import a3 from './3.vue'
import a4 from './4.vue'
import a5 from './5.vue'


export default {
  name: 'Header',
  methods: {
    visablePage: function (e) {
      let n = e.target.attributes[1].nodeValue.split('n')[1]-1
      a1.chenge(arr[0][n])
      a2.chenge(arr[1][n])
      a3.chenge(arr[2][n])
      a4.chenge(arr[3][n])
      a5.chenge(arr[4][n])
    }
  }
}

let arr=[
  [1,0,0,0,0],
  [0,1,0,0,0],
  [0,0,1,0,0],
  [0,0,0,1,0],
  [0,0,0,0,1]
]
</script>

<style scoped>

button{
  align-items: center;
  padding: 0px;
  margin:3px;
  width:50px;
  height:25px;
  font-family: -apple-system, BlinkMacSystemFont, 'Roboto', sans-serif;
  border-radius: 6px;
  border:none;


  background: #6E6D70;
  box-shadow: 0px 0.5px 1px rgba(0, 0, 0, 0.1), inset 0px 0.5px 0.5px rgba(255, 255, 255, 0.5), 0px 0px 0px 0.5px rgba(0, 0, 0, 0.12);
  color: #ffffff;

}

button:focus {
  box-shadow: inset 0px 0.8px 0px -0.25px rgba(255, 255, 255, 0.2), 0px 0.5px 1px rgba(0, 0, 0, 0.1), 0px 0px 0px 3.5px rgb(99, 99, 99);
  outline: 0;
  color: #000000;
}

.b1{background:#4CAF50}
.b2{background:#008CBA}
.b3{background:#f44336}
.b4{background:#dadada}
.b5{background:#6E6D70}

.header{
  display:block;
  box-sizing: content-box;
  width:100%;
  background: #6E6D70;
}
</style>

