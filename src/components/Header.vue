<template>
    <header>
        <img src="../assets/logo.png" alt="logo-fable">
        <ul>
            <li v-for="(element, index) in headerElements" :key="`list-${index}`">
                <img :src="require(`@/assets/${element.img}`)" :alt="element.img">
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

<style>

</style>