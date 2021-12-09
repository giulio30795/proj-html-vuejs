<template>
    <header class=" container d-flex justify-content-center align-items-center">
        <img class="logo" src="../assets/logo.png" alt="logo-fable">
        <ul class="list-unstyled d-flex mb-0">
            <li class=" d-flex flex-column align-items-center py-3 px-2" v-for="(element, index) in headerElements" :key="`list-${index}`">
                <img class="mb-1" :src="require(`@/assets/${element.img}`)" :alt="element.img">
                <h4>{{element.text}}</h4>
            </li>
        </ul>
    </header>
</template>

<script>

import HeaderMenu from '@/DevData/HeaderMenu.js'
export default {
name: 'Header',
data(){
    return {
        headerElements: HeaderMenu,
    }
},

}

</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

li {
    height:100%;
    width:80px;
    cursor: pointer;
    &:hover{
        transition: .3s;
        background-color: $main;
        &:hover h4{
            transition: .3s;
            color:white;
        }
        &:hover img{
            transition: .3s;
            filter: brightness(100)
        }
    }
    img{
        width:20px;
    }
}
.logo {
    width: 120px;
    height:100%;
    margin-right: 80px;
    cursor:pointer;
}
h4{
    font-size: .7rem;
    font-weight: 200;
    color: $secondary;
    margin: 5px 0;
    font-family: 'Lato', sans-serif;

}
</style>