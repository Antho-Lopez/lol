<template>
  <div class="champions">
   <Champion v-for="champion in champions" :key="champion.id" :champion="champion"/>
  </div>
</template>

<script>
import Champion from './Champion.vue'

export default {
  name: 'Champions',
  props: {
    champions: Array
  },
  components: {
    Champion
  }
} 
</script>

<style scoped>

.champions{
  display: flex;
  flex-direction: column;
}

</style>