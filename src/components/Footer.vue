<template>
  <footer>
    <p>{{copyright}}</p>
  </footer>
</template>

<script>

export default {
  data:function() {
    return {
      copyright: 'copyright 2018 vue ninjas'
    };
  }
}

</script>

<style scoped>
  footer{
    background: #222;
    padding: 6px;
  }
  p{
    color: lightgreen;
    text-align: center;
  }
</style>
