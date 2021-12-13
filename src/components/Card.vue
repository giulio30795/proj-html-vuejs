<template>
    <div class="col-4 px-4">
        <div class="grey my-3">October 03, 2014</div>
        <div class="rel"> 
            <img :src="img" alt="Bambini">
            <div class="box d-flex justify-content-center align-items-center">{{number}}</div>
        </div>
        <h5 class="my-2">{{titleCard}}</h5>
        <p class="grey">Magna est consectetur interdum modest dictum. Curabitur est faucibus, malesuada esttincidunt etos et mauris, nunc a libero govum est cuprum [...]</p>
        <span>
            <img src="../assets/images/author.png" alt="">
            <span>Anna Brown</span>
        </span>
        <span>
            <img src="../assets/images/category.png" alt="">
            <span>{{role}}</span>
        </span>
    </div>
</template>

<script>
export default {
name: 'Card',

props: {
    img: String,
    number: Number,
    titleCard: String,
    role: String,

},
}
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

.grey{
    color: $text-grey;
    font-size: 1rem;
}
.box{
    height: 35px;
    width:35px;
    background-color: $main;
    color:white;
    position: absolute;
    bottom: 0;
    right: 0;
}

.rel{
    position: relative;

}
span{
    color: $text-grey;
    margin: 0 10px;
    vertical-align: center;
}
h5{
    color: $secondary;
    font-weight:300;
    font-size: 1.4rem;
}
p{
    padding:10px 0;
    margin: 0;
    border-bottom: .2px solid $text-grey;
    margin-bottom: 5px;
}
img{
    max-width: 100%;
}

</style>