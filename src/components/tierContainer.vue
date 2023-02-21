<script>
import characterContainer from './characterContainer.vue';

export default {
    components: {
        characterContainer
    },
    props: ["tier", "characters"],
}
</script>

<template>

    <div class="tierContainer">
        <h2>{{ tier }}</h2>
        <characterContainer v-for="character in characters" :key="character.name" :name="character.name"/>

    </div>

</template>

<style scoped lang="scss">
  .tierContainer {
    width: calc(100% - 40px);
    margin: 20px;
    background-color: rgba(255, 255, 255, 0.1);
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;

    h2 {
      height: 150px;
      aspect-ratio: 1 / 1;
      background-color: rgba(255, 255, 255, 0.1);
      margin: 10px;
      text-align: center;
      line-height: 100px;
      font-size: 32px;
    }
  }

</style>