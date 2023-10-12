<script>
import { store } from '../data/store';
import CharacterCard from './partials/CharacterCard.vue';
export default {
  nome: 'CardsContainer',
  components:{
    CharacterCard
  },
  data (){
    return{
      store
    }
  },
  mounted(){
    console.log(store.charctersList);
  }
}
</script>


<template>
  <div class="container my-5">
    <div class="row">
      <CharacterCard
        v-for="character in store.charctersList"
        :key="character.id"
        :image="character.image"
        :name="character.name"
      />
    </div>
  </div>
</template>


<style lang="scss" scoped>

</style>