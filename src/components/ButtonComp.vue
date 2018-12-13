<template>
  <!-- Your HTML goes here -->
  <div>
    <h1 v-bind:title="message"> Hello {{ person.firstname}} qui vient de {{from}}</h1>
    
    <button v-on:click="seen = !seen">Vue.JS</button>
    <p v-if="seen">Maintenant vous me voyez</p>
  </div>

</template>

<script>
  /* Your JS goes here */
  export default {
  name: 'ButtonComp',
  data () {
    return {
      person: {
          firstname: 'Homer',
          lastname: 'Simpson'
      },
      from:'Springfield',
      message:'Vous avez affiché cette page le ' + new Date().toLocaleString(),
      seen:false,
      
    }
  }
  // methods: {
  //   reverseMessage: function () {
  //     // this.message = this.message.split('').reverse().join('')
  //      seen==true ? seen:false : seen:true
  //   }
  // }
}
</script>

<style>
  button{
    border:none;
    background:lightsalmon;
    color:lemonchiffon;
    padding:10px 25px;
    cursor:pointer;
  }
</style>