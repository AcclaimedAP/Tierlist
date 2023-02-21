<script>
export default {
    props: {
        name: {
            type: String,
            default: "Not Found"
        }
    }
}
</script>
<template>
        <div class="characterPortrait">
            <div class="imageContainer">
                <img src="/public/mockimage/portrait.webp" alt="placeholder image">
            </div>
            <h3>{{ name }}</h3>
        </div>
</template>

<style scoped lang="scss">
    .characterPortrait {
        background-color: rgba(255, 255, 255, 0.1);
        margin: 10px;
        max-height: 150px;
        height: 150px;
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
</style>