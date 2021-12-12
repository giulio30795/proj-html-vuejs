<template>
    <section class="py-4">
        <div
            class="container pt-5 d-flex justify-content-center align-items-center flex-column"
        >
            <div
                class="circle d-flex justify-content-center align-items-center"
            >
                <img src="../assets/images/quote_alt.png" alt="" />
            </div>
            <p class="pb-2 pt-4 fs-2 text-center">
                Fable Kindergarten is a great place for my daughter to start her
                schooling experience. It's welcoming and safe and my daughter
                loves being there.
            </p>
            <div class="mb-3">________</div>
            <div class="pt-2 pb-3">Joe R. Hamblen</div>
        </div>
        <div class="container d-flex justify-content-center py-4">
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
export default {
    name: "FablePlace",
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

section {
    background-image: url("../assets/images/parallax_02.jpg");
    background-position: center;
    background-size: cover;
    color: white;
}
p {
    padding: 0 100px;
    font-weight: 100;
}
.circle {
    height: 100px;
    width: 100px;
    border-radius: 50px;
    border: 1px solid white;
    padding: 10px;
    img {
        width: 50px;
    }
}

.square {
    width: 40px;
    height: 10px;
    border: 2px solid white;
    margin: 0 8px;
}

.square:nth-child(4) {
    transform: translateY(-10px);
}
</style>
