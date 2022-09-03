<template>
    <div>
        <button>Add hat</button>
        <div class="hatListItem">
            <div>Hat name 1</div>
            <img class="pixelart" src="./testHat.png">
        </div>
        <div class="hatListItem">
            <div>Hat name 2</div>
            <img class="pixelart" src="./testHat.png">
        </div>
    </div>
</template>

<script>
export default{
    data() {
        return{
            likes: 0,
            dislikes: 0,
        }
    },
    methods: {
        addLike() {
            this.likes++;
        },
        addDislike(){
            this.dislikes++;
        }
    }
}
</script>

<style scoped>
*{
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}

.pixelart {
    width: 250px;
    background-image: url('ducks.png');
    background-color: white;
    background-repeat: no-repeat;
    background-size: cover;
    image-rendering: pixelated;
    image-rendering: -moz-crisp-edges;
    image-rendering: crisp-edges;
    border: 2px solid yellow;
}

.hatListItem{
    padding: 15px;
    border: 2px solid yellow;
    margin-top: 15px;
    background-color: palegoldenrod;
}
</style>