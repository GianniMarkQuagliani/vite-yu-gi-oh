<script>
export default {
  nome: 'CharacterCard',
  props:{
    image: String,
    name: String
  }
}
</script>


<template>
  <div class="col-3">
    <div class="sc-card">
      <img :src="image" :alt="name">
    </div>
  </div>
</template>


<style lang="scss" scoped>

</style>