<script>
export default {
  name: 'CharacterCard',
  props:{
    image: String,
    name: String,
    archetype: String
  }
}
</script>


<template>
      
<div class="col-3">
  <div class="card">
    <img class="card-img-top" :src="image" :alt="name">
    <div class="card-body">
      <p>{{name}}</p>
      <p>{{archetype}}</p>
     </div>
  </div>
</div>
      
</template>


<style lang="scss" scoped>
.card{
  margin-bottom: 50px;
}

</style>