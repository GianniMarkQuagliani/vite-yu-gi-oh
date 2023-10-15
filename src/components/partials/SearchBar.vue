<script>
import { store } from '../../data/store';
export default {
    name: 'SearchBar',
    data(){
        return{
            store
        }
    },
    methods :{
        reset (){
            store.nameToSearch = '';
            store.archetypeToSearch = '';
            this.$emit('startSearch');
        }
    }
}
</script>


<template>
  <div class="container">
    <div class="row justify-content-center">
        <div class="col-auto">
            <input v-model="store.nameToSearch" type="text" class="form-control" placeholder="Search">
        </div>
        <div class="col-auto">
            <select v-model="store.archetypeToSearch" name="form-control" aria-label="Default select example">
                <option selected value="">Select archetype</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
            </select>
        </div>
        <div class="col-auto">
            <button @click="$emit('startSearch')" class="btn btn-info">Search</button>
        </div>
        <div class="col-auto">
            <button class="btn btn-warning">Reset</button>
        </div>
    </div>
  </div>
</template>



<style lang="scss" scoped>

</style>