<template>
    <div>
        <Divider :Title="Title5" :Subtitle="Subtitle5" />
        <div class="container d-flex justify-content-center px-5">
            <ContactCard
                v-for="(element, index) in ContactList"
                :key="`contact-${index}`"
                :img="element.img"
                :title="element.title"
                :info1="element.info1"
                :info2="element.info2"
                :info3="element.info3"
            />
        </div>
        <div class="container d-flex justify-content-center px-5">
            <div
                class="col-6 mt-5 px-4 d-flex flex-column justify-content-between"
            >
                <input type="text" placeholder="Your Name*" />
                <input class="" type="email" placeholder="Your Email*" />
                <input type="text" placeholder="Subject" />
            </div>
            <div class="col-6 mt-5 px-4">
                <textarea
                    name=""
                    placeholder="Your Message*"
                    id=""
                    cols="50"
                    rows="6"
                ></textarea>
            </div>
        </div>
        <div class="d-flex justify-content-center py-4">
            <div
                class="bottone d-flex justify-content-center align-items-center"
            >
                <span>Go To Blog</span>
                <img src="../assets/images/slider_next.png" alt="next" />
            </div>
        </div>
    </div>
</template>

<script>
import ContactList from "@/DevData/ContactList.js";
import ContactCard from "./ContactCard.vue";
import Divider from "./Divider.vue";

export default {
    name: "ContactUs",
    components: {
        ContactCard,
        Divider,
    },
    data() {
        return {
            ContactList: ContactList,
            Title5: "Contact Us",
            Subtitle5: "Our postal addres and contact details",
        };
    },
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

input,
textarea {
    border: 0.1px solid $text-grey;
}
.bottone {
    font-size: 0.8rem;
    font-weight: 400;
    padding: 5px 4px 5px 11px;
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
