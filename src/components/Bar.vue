<template>
    <div class="bar">
        <div class=" container d-flex justify-content-evenly py-5 align-items-center">
            <div class="text">
                {{MainText}}
            </div>
            <div class="button">
                <a href="#">{{ButtonText}}</a>
                <img src="../assets/images/slider_next.png" alt="">
                
            </div>
        </div>
    </div>
</template>

<script>
export default {
name: 'Bar',

props:{
    MainText: String,
    ButtonText: String,
}
}
</script>

<style scoped lang="scss">
.bar{
    background-image: url('../assets/images/pattern.png');
    color:white;
    }
.text{
    font-size: 1.5rem;
    font-weight: 100;
}
.button{
    border: 1px solid white;
    text-transform: uppercase;
    padding: 5px 0px 5px 15px;
}
a{
    color: white;
    text-decoration: none;
    &:hover{
        color: currentcolor;
    }
}
</style>