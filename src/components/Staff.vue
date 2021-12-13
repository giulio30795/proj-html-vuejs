<template>
    <div class="container px-5">
        <div class="row justify-content-center pe-2">
            <div class="col-6 px-5">
                <h3>
                    Our staff consists of three teachers and one assistant with
                    experience in early childhood care.
                </h3>
            </div>
            <div class="col-6 px-5">
                <p>
                    Praesent arcu gravida vehicula est node maecenas loareet
                    morbi a dosis luctus. Urna eget lacinia eleifend praesent
                    luctus a arcu quis facilisis venenatis. Aenean interdum,
                    nibh vitae sodales, magna ante feugiat elit maecenas.
                </p>
            </div>
        </div>

        <ul class="row justify-content-center flex-wrap list-unstyled">
            <li
                v-for="(element, index) in StaffList"
                :key="`Class-${index}`"
                class="col-6 mx-0 px-5 my-3"
            >
                <div class="row">
                    <div
                        class="img-container col-6 d-flex justify-content-between flex-column"
                    >
                        <img
                            :src="require(`../assets/images/${element.img}`)"
                            alt="Teacher"
                        />
                        <div
                            class="plus d-flex justify-content-center align-items-center"
                        >
                            <img
                                src="../assets/images/image_overlay.png"
                                alt="overlay"
                            />
                        </div>
                        <div class="text-center mt-3">
                            <h6>
                                {{ element.name }}
                            </h6>
                            <div class="text">
                                {{ element.role }}
                            </div>
                        </div>
                    </div>
                    <div class="col-6 d-flex justify-content-end flex-column">
                        <div class="description">
                            <div class="box">
                                <img src="../assets/images/quote.png" alt="" />
                            </div>
                            {{ element.description }}
                        </div>
                        <div class="d-flex mt-2">
                            <span
                                class="d-flex justify-content-center align-items-center"
                            >
                                <img
                                    :src="
                                        require(`../assets/images/${element.social_1}`)
                                    "
                                    alt="Teacher"
                                />
                            </span>
                            <span
                                class="d-flex justify-content-center align-items-center"
                            >
                                <img
                                    :src="
                                        require(`../assets/images/${element.social_2}`)
                                    "
                                    alt="Teacher"
                                />
                            </span>
                            <span
                                class="d-flex justify-content-center align-items-center"
                            >
                                <img
                                    :src="
                                        require(`../assets/images/${element.social_3}`)
                                    "
                                    alt="Teacher"
                                />
                            </span>
                        </div>
                    </div>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
import StaffList from "@/DevData/StaffList.js";
export default {
    name: "Staff",
    data() {
        return {
            StaffList: StaffList,
        };
    },
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";
h6 {
    color: $secondary;
    font-weight: 200;
}
.text {
    color: $text-grey;
    font-weight: 150;
}
li {
    margin-right: 1px;
}
.img-container > img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}
.description {
    font-size: 0.85rem;
    position: relative;
    color: $text-grey;
    font-weight: 300;
    .box {
        width: 100px;
        height: 50px;
        border: 2px solid $main;
        position: absolute;
        bottom: 135px;
        left: -50px;
        text-align: right;
        vertical-align: middle;
        padding: 10px 10px 0 0;
        img {
            width: 30%;
        }
    }
}
.img-container {
    position: relative;
    cursor: pointer;
    &:hover .plus {
        opacity: 0.5;
    }
}
.plus {
    width: 80px;
    height: 80px;
    border-radius: 40px;
    background-color: $secondary;
    position: absolute;
    left: 50%;
    top: 35%;
    transform: translate(-50%, -50%);
    opacity: 0;
    transition: all 0.3s;
}
span {
    background-color: $main;
    margin-right: 2px;
    margin-top: 20px;
}
h3,
h4 {
    color: $secondary;
    font-weight: 300;
}
p {
    color: $text-grey;
}
</style>
