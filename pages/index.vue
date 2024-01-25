<script setup>
const open = ref(false)
const textButton = ref('Show modal')
const toggle = () => {
    open.value = !open.value
    textButton.value = open.value ? 'Hide modal' : 'Show modal'
}
</script>
<template>
    <div class="textBait">
        <h3>Odkryj urok fryzur w naszym ekskluzywnym salonie

            <div class="line-2"></div>
        </h3>
        <img src="./azjatka UwU 1.png" alt="" />
    </div>
    <button @click="toggle">{{ textButton }}</button>
    <div v-if="open">To jest ukryty tekst</div>
    <div class="wrapped">
        <div class="reservation">
            <div class="wide1">
                <div class="centered">
                    ZAREZERWUJ WIZYTĘ
                </div>
            </div>
            <img src="./greg-trowman-jsuWg7IXx1k-unsplash 1.png" alt="" class="wide" />

        </div>
    </div>
    <div class="line-3"></div>
    <br />




    <div class="titleGallery"> Galeria</div>
    <br />
    <br />
    <div class="gallery">
        <div class="sideLeft">
            <img src="./nora-hutton-ZhrGA3iTpPk-unsplash 2.png" alt="" />
        </div>
        <div class="centeredImage">
            <img src="./delfina-pan-wJoB8D3hnzc-unsplash 1.png" alt="">
        </div>
        <div class="sideRight">
            <img src="./nora-hutton-ZhrGA3iTpPk-unsplash 1.png" alt="">
        </div>
    </div>
    <div class="line-4"></div>
</template>
<style scoped lang="scss">
h3 {
    font-family: vladimir script;
    font-size: 80px;
    display: flex;
    justify-content: left;
    flex-direction: column;
    float: right;
    position: relative;
    right: 20px;
    top: 100px;
}

.line-2 {
    height: 1px;
    background: black;
    position: relative;
    top: 10px;
    z-index: 99;


    width: 100%;
}

.line-3 {
    height: 84px;
    background: #DCA86F;
    position: relative;
    top: 0px;
    z-index: 99;


    width: 100%;
}

.line-4 {
    height: 7px;
    background: #DCA86F;
    position: relative;
    width: 100%;
    top: -350px;
    z-index: -1;



    width: 100%;
}


img {
    width: 20%;
    position: relative;



}

.reservation {
    display: grid;
}

.centered {

    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    width: 50%;
    height: 50%;


    border: solid white;
    font-size: 80px;

}

.wide {
    width: 100%;

    grid-column: 1;
    grid-row: 1;

}

.wide1 {
    z-index: 9999;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    grid-column: 1;
    grid-row: 1;
}

.textBait {
    width: 100%;
    height: 400px;
}

.gallery {
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-wrap: 100px;

    img {
        width: 122%;
    }


}

.titleGallery {
    font-family: vladimir script;
    font-size: 80px;
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>