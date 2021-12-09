<template>
    <div class="jumbo">
        <div class="container">
            <div class="text">Learning e Fun</div>
            <img class="gioco1" src="../assets/images/slider_slide3_img2.png" alt="treno">
            <img class="gioco2" src="../assets/images/slider_slide3_img3.png" alt="giochi">
            <div class="box1"></div>
            <div class="box2"></div>
            <div class="box3"></div>
        </div>
    </div>
</template>

<script>
export default {
name: 'Jumbo'
}
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

.jumbo{
    width:100%;
    height:500px;
    background-image: url('../assets/images/slider_slide3_background.png');
}

.container{
    height:100%;
    background-position: bottom;
    position: relative;
    font-family: 'Handlee' , cursive;
}
.text{
    color: $main;
    position: absolute;
    left: 280px;
    top: 120px;
    opacity: .1;
    font-size: 1.4rem;
}
.gioco1{
    position:absolute;
    bottom:50px;
    left:500px
}

.gioco2{
    position:absolute;
    bottom:50px;
    left:1000px;
}

.box1, .box2, .box3{
    border: 1px solid $main;
    width: 40px;
    height: 10px;
    position: absolute;
}

.box1{
    bottom: 30px;
    left:620px;
}

.box2{
    bottom: 30px;
    left:670px;
}

.box3{
    bottom: 40px;
    left:720px;
}

</style>