<template>
    <section class="py-5">
        <ul class="list-unstyled container d-flex justify-content-center">
            <li
                class="col-2 text-center d-flex flex-column justify-content-start align-items-center"
                v-for="(element, index) in NumberElements"
                :key="`number-${index}`"
            >
                <div class="d-flex justify-content-center align-items-center">
                    {{ element.number }}
                </div>
                <h5 class="my-3">{{ element.title }}</h5>
                <p>{{ element.text }}</p>
            </li>
        </ul>
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
}

div {
    width: 100px;
    font-size: 2rem;
    font-weight: 100;
    height: 100px;
    border-radius: 50px;
    vertical-align: middle;
    border: 1px solid white;
}

</style>
