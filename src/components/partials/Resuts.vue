<script>
import { store } from '../../data/store';
export default {
  nome: 'Results',
  data(){
    return{
      store
    }
  },
  computed:{
    outputResult(){
      return 'risultati trovati: ' + store.charctersList.length
    }
  }
}
</script>


<template>
  <p>{{outputResult}}</p>
</template>


<style lang="scss" scoped>

p{
  margin-bottom: 50px;
  text-align: center;
  color: green;
  font-weight: bold;
  font-size: large;
  background-color: white;
  width: 200px;
  margin: auto;
}
</style>