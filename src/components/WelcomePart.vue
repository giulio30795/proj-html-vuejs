<template>
    <ul class="container d-flex justify-content-center list-unstyled px-4">
        <li class="col-3 text-center d-flex flex-column justify-content-start align-items-center px-3"
        v-for="(element, index) in WelcomeList" :key="`welcome-${index}`">
            <div class="d-flex justify-content-center align-items-center">
                <img :src="require(`../assets/images/${element.img}`)" alt="element.title">
            </div>
            <h4 class="my-4">{{element.title}}</h4>
            <p class="px-3">{{element.text}}</p>
        </li>
    </ul>
</template>

<script>

import WelcomeList from '@/DevData/WelcomeList.js'
export default {
name: 'WelcomePart',

data(){
    return {
        WelcomeList: WelcomeList,
    }
},
}
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

ul li:first-child div, ul li:nth-child(3) div{
    background-color: $main;
    img{
        filter: brightness(100);
        color:white;
    }
}

ul li:last-child div, ul li:nth-child(2) div{
    background-color: $secondary;
}
div{
    width:180px;
    height: 180px;
    border-radius: 90px;
    vertical-align: middle;
}
img{
    width: 50px;
}
h4{
    color: $secondary;
    font-weight: 200;
}
p{
    color: $text-grey;
}
</style>