<template>
    <div class="bar">
        <div
            class="container d-flex justify-content-around align-items-center"
        >
            <div class="text">
                {{ MainText }}
            </div>
            <div class="button">
                <a href="#">{{ ButtonText }}</a>
                <i class=" mx-3 fas fa-angle-right"></i>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Bar",

    props: {
        MainText: String,
        ButtonText: String,
    },
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";
.bar {
    background-image: url("../assets/images/pattern.png");
    color: white;
    padding: 30px 0;
}
.text {
    font-size: 2.3rem;
    font-weight: 100;
}
.button {
    border: 1px solid white;
    text-transform: uppercase;
    padding: 7px 0px 5px 15px;
    transition: all 0.3s;
    &:hover{
        background-color: white;
        cursor:pointer;
        &:hover a {
            color: $secondary;
        }
        &:hover i {
            color: $secondary;
        }
    }

}
a {
    color: white;
    text-decoration: none;
}
</style>
