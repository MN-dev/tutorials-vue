<template>
<div>
  <form-helper>
    
    <div slot="form-header">
      <h1>Form tow login </h1>
      <p>Enter your login credintals </p>
    </div>

    <div slot="form-fields">
      <input type="text" placeholder="username" required>
      <input type="password" placeholder="password" required>
      
    </div>

      <div slot="form-controls">
        <button v-on:click="handelSubmit">send</button>
      </div>      
     <div id="useful-links">
    <u>
      <li><a href="#">link1</a></li>
      <li><a href="#">link2</a></li>
      <li><a href="#">link3</a></li>
      <li><a href="#">link4</a></li>
    </u>
    </div>
   

</form-helper>
</div>
</template>

<script>
  import formHelper from './formHelper.vue'
  export default{
    components:{
      'form-helper':formHelper
    },
    data(){
      return{
        counter:0
      }
    },
    methods:{
      handelSubmit:function(){
        alert('thanks for logging in (form tow)');
      }
    }

  }
  
</script>

<style scoped>

h1{
  text-align: center;
}
form{
  width: 100%;
  max-width: 960px;
  margin: 0 auto;
}
#useful-links ul{
  padding: 0;
}
#useful-links li{
  display: inline-block;
  margin-right: 10px;
}
form > div{
  padding: 20px;
  background: #eee; 
  margin: 20px 0;
}

#form-header{
  background: #ddd;
  border: 1px solid #bbb;
}

</style>