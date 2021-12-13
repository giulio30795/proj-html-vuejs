<template>
    <div class="container text-center my-5">
        <h2>{{ Title }}</h2>
        <p>{{ Subtitle }}</p>
        <img src="../assets/images/header_divider.png" alt="divider" />
    </div>
</template>

<script>
export default {
    name: "Divider",

    props: {
        Title: String,
        Subtitle: String,
    },
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

h2 {
    color: $secondary;
    font-size: 3rem;
    font-weight: 100;
}

p {
    color: $text-grey;
}
</style>
