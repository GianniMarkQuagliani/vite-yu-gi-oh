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
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
      <div class="col-3">
        <CharacterCard />
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>

</style>