<template>
<div>
  <keep-alive>
    <component v-bind:is="component"></component>
  </keep-alive>
  <button v-on:click="component = 'form-one'">Show form one</button>
  <button v-on:click="component = 'form-tow'">Show form tow</button>
</div>
</template>
<script>
import formOne from'./components/formOne.vue'
import formTow from'./components/formTow.vue'

export default {
  components:{
    'form-tow':formTow,
    'form-one':formOne
  },

  data(){
    return{
      component:'form-one'
    }
  },
  methods:{}
  }

</script>

<style >
</style>
