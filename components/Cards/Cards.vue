<template>
    <div style="display: flex; gap: 5px;">
      <div v-for="item in tableauCards" :key="item.title"  style="border: 1px solid black;  padding: 10px">
        <p>{{ item.title }}</p>
        <p>{{ item.description }}</p>
        
    </div>
    </div>
</template>

<script setup lang="ts">
import  {CardsDto}  from '../../models/cardsDto';
  const tableauCards = ref<CardsDto[]>([
    {title: 'Carte 1', description: 'Description de la carte 1'},
    {title: 'Carte 2', description: 'Description de la carte 2'}
  ])  

</script>