<template>
    <section class="py-5">
        <ul class="list-unstyled container d-flex justify-content-center py-3">
            <li
                class="col-2 text-center d-flex flex-column justify-content-start align-items-center"
                v-for="(element, index) in NumberElements"
                :key="`number-${index}`"
            >
                <span class="d-flex justify-content-center align-items-center">
                    {{ element.number }}
                </span>
                <h5 class="my-4">{{ element.title }}</h5>
                <p>{{ element.text }}</p>
            </li>
        </ul>
        <div class="container d-flex justify-content-center py-3">
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
        </div>
    </section>
</template>

<script>
import NumbersList from "@/DevData/NumbersList.js";
export default {
    name: "Numbers",

    data() {
        return {
            NumberElements: NumbersList,
        };
    },
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";
section{
    color: white;
    background-image: url('../assets/images/parallax_01.jpg');
    background-position: center;
}

li span {
    width: 150px;
    height: 150px;
    font-size: 2rem;
    font-weight: 100;
    border-radius: 75px;
    vertical-align: middle;
    border: 2px solid white;
}

.square{
    width: 40px;
    height: 10px;
    border: 2px solid white;
    margin: 0 8px;
}

.square:first-child{
    transform: translateY(-8px);
}

</style>
