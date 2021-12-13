<template>
    <div class="container">
        <div>
            <Divider :Title="Title4" :Subtitle="Subtitle4" />
        </div>
        <div class="d-flex justify-content-center">
            <Card
                :img="img1"
                :number="number1"
                :titleCard="titleCard1"
                :role="role1"
            />

            <Card
                :img="img2"
                :number="number2"
                :titleCard="titleCard2"
                :role="role2"
            />

            <Card
                :img="img3"
                :number="number3"
                :titleCard="titleCard3"
                :role="role3"
            />
        </div>

        <div class="d-flex justify-content-center py-4">
            <div
                class="bottone d-flex justify-content-center align-items-center"
            >
                <span> Read More </span>
                <img src="../assets/images/slider_next.png" alt="next" />
            </div>
        </div>
    </div>
</template>

<script>
import Divider from "./Divider.vue";
import Card from "./Card.vue";
export default {
    name: "WhatsNew",

    components: {
        Divider,
        Card,
    },

    data() {
        return {
            Title4: "What's New",
            Subtitle4: "Keep up to date with the latest news",
            img1: require("../assets/images/blog_09.jpg"),
            number1: 42,
            titleCard1: "Drawing and Painting Lessons",
            role1: "Event's Fun",
            img2: require("../assets/images/blog_10.jpg"),
            number2: 19,
            titleCard2: "Fall Parents Meeting Day",
            role2: "Dance, Education",
            img3: require("../assets/images/blog_08.jpg"),
            number3: 22,
            titleCard3: "Birthday in Kindergarten",
            role3: "Games, General",
        };
    },
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

.bottone {
    font-size: 0.8rem;
    font-weight: 400;
    padding: 5px 5px 5px 12px;
    background-color: $main;
    color: white;
    text-transform: uppercase;
    width: 120px;
    height: 50px;
    img {
        width: 25px;
    }
}
</style>
