<template>
    <div class="container  d-flex justify-content-center flex-column align-itemr-center py-4">
        <div class="d-flex justify-content-center mb-3">
            <span class="d-flex justify-content-center align-items-center">
                <img src="../assets/images/behance.png" alt="Teacher">
            </span>
            <span class="d-flex justify-content-center align-items-center">
                <img src="../assets/images/dribbble.png" alt="Teacher">
            </span>
            <span class="d-flex justify-content-center align-items-center">
                <img src="../assets/images/envato.png" alt="Teacher">
            </span>
            <span class="d-flex justify-content-center align-items-center">
                <img src="../assets/images/facebook.png" alt="Teacher">
            </span>
            <span class="d-flex justify-content-center align-items-center">
                <img src="../assets/images/twitter.png" alt="Teacher">
            </span>
        </div>
        <div class="text-center">
            Fable - Children Kindergarten WordPress Theme by QuanticaLabs
        </div>
    </div>
</template>

<script>
export default {
name: 'Social'
}
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";


span{
    background-color: $main;
    margin: 0 1px;
    width: 50px;
    height: 50px;
}

div:last-child div {
    color: $text-grey;
}
</style>