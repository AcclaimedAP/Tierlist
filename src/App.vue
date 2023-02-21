<script>
import tierContainer from './components/tierContainer.vue';

export default {
  data() {
    return {
      tiers: ['S+', 'S', 'A', 'B', 'C', 'D', 'Unranked'],
      characters: [
        {
        name: "keqing"
        },
        {
        name: "qiqi"
        },
        {
        name: "mona"
      }
      ]
    }
  },
  components: {
    tierContainer
  }
}
</script>

<template>
  <div class="container"><h1>Tier list</h1>
    <tierContainer v-for="tier in tiers" :key="tier.tiers" :tier="tier" :characters="characters"/>
  
  </div>
</template>

<style scoped lang="scss">
.container {
  background-color: rgba(255, 255, 255, 0.1);
  width: 80vw;
  position: fixed;
  top: 5vh;
  left: 10vw;
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  height: 90vh;
  overflow: scroll;
  h1 {
    text-align: center;
  }


}
</style>
