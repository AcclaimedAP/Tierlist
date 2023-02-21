<script>
export default {
    props: ['tier']
}
</script>

<template>

    <div class="tierContainer">
        <h2>{{ tier }}</h2>
        <div class="characterPortrait">
            <div class="imageContainer">
                <img src="https://api.genshin.dev/characters/qiqi/portrait" alt="placeholder image">
            </div>
            <h3>Qiqi</h3>
        </div>
        <div class="characterPortrait">
            <div class="imageContainer">
                <img src="https://api.genshin.dev/characters/qiqi/portrait" alt="placeholder image">
            </div>
            <h3>Qiqi</h3>
        </div>
        <div class="characterPortrait">
            <div class="imageContainer">
                <img src="https://api.genshin.dev/characters/qiqi/portrait" alt="placeholder image">
            </div>
            <h3>Qiqi</h3>
        </div>
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
    .characterPortrait {
        background-color: rgba(255, 255, 255, 0.1);
        margin: 10px;
        .imageContainer {
            max-height: 100px;
            overflow: hidden;
            img {
                max-height: 200px;
            }
        }
        h3 {
            margin: 5px;

        }
    }


    h2 {
      height: 140px;
      aspect-ratio: 1 / 1;
      background-color: rgba(255, 255, 255, 0.1);
      margin: 10px;
      text-align: center;
      line-height: 100px;
      font-size: 32px;
    }
  }

</style>