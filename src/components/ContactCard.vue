<template>
    <div class="col-2 text-center">
        <img :src="img" alt="Contact-img">
        <h5 class="my-3">{{title}}</h5>
        <div>{{info1}}</div>
        <div>{{info2}}</div>
        <div>{{info3}}</div>
    </div>
</template>

<script>
export default {
name: 'ContactCard',
props:{
    img: String,
    title: String,
    info1: String,
    info2: String,
    info3: String,
},
}
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

h5{
    color: $secondary;
    font-weight: 300;
}
div > div {
    color: $text-grey;
}

</style>