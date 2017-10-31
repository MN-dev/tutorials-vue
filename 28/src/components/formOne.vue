<template>
<div>
  <form-helper>
    <form>
      <h1>Please fill out our form ...</h1>
    <div slot="form-header">
      <h1>Form one - Contact us </h1>
      <p>Fill in this form to Contact us </p>
    </div>

    <div slot="form-fields" >
      <input type="text" placeholder="name" required>
      <label>your message</label>
      <textarea></textarea>
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
  </form>
</form-helper>
</div>
</template>

<script>
  import formHelper from './formHelper.vue'
  
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