<template>
  <div id="ninjas">
    <ul>
      <li v-for="x in ninjas" v-on:click="x.show=!x.show">
        <h2>{{x.name}}</h2>
        <h3 v-show="x.show">{{x.speciality}}</h3>
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  data:function() {
    return {
      ninjas:[
        {name:'Ryu',speciality:'Vue components',show:false},
        {name:'Crystal',speciality:'HTML wizardry',show:false},
        {name:'Hitoshi',speciality:'Click Events',show:false},
        {name:'Tango',speciality:'Conditionals',show:false},
        {name:'Kami',speciality:'Webpack',show:false},
        {name:'Yoshi',speciality:'Data diggin',show:false}
      ]
    };
  }
}

</script>

<style scoped>
  #ninjas{
    width: 100%;
    max-width: 1200px;
    margin: 40px auto;
    padding: 0 20px;
    box-sizing: border-box;
  }
  ul{
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
  }
  li{
    flex-grow: 1;
    flex-basis: 300px;
    text-align: center;
    padding: 30px;
    border: 1px solid #222;
    margin: 10px;
  }
</style>
