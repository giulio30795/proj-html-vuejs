<template>
    <section class="container pb-4">
        <div class="row justify-content-center px-2">
            <div class="col-6 px-5">
                <h3 class="title ps-4">
                    We provided four classes with nine to twenty children each
                    aged twelve month to five years of age.
                </h3>
            </div>
            <div class="col-6 ps-4 pe-5">
                <p class="description pe-2">
                    Praesent arcu gravida vehicula est node maecenas loareet
                    morbi a dosis luctus. Urna eget lacinia eleifend praesent
                    luctus a arcu quis facilisis venenatis. Aenean interdum,
                    nibh vitae sodales, magna ante feugiat elit maecenas.
                </p>
            </div>

            <ul class="row justify-content-center flex-wrap list-unstyled px-5">
                <li
                    v-for="(element, index) in ClassElement"
                    :key="`class-${index}`"
                    class="col-6 mx-0 d-flex px-4 my-3"
                >
                    <div
                        class="left d-flex flex-column w-50 justify-content-between p-3"
                    >
                        <div>
                            <div class="fs-5">{{ element.title }}</div>
                            <div class="grey">{{ element.subtitle }}</div>
                        </div>
                        <div class="d-flex justify-content-around">
                            <div class="box-border">
                                <div class="text-center">
                                    {{ element.age }}
                                </div>
                                <div class="grey">{{ element.old }}</div>
                            </div>
                            <div>
                                <div class="text-center">
                                    {{ element.class_size }}
                                </div>
                                <div class="grey">
                                    {{ element.class }}
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="right w-50">
                        <img
                            :src="require(`../assets/images/${element.img}`)"
                            alt="Bambini"
                        />
                        <div>
                            <div
                                class="d-flex justify-content-center align-items-center"
                            >
                                <span> Read More </span>
                                <img
                                    src="../assets/images/slider_next.png"
                                    alt="next"
                                />
                            </div>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
import ClassList from "@/DevData/ClassList.js";
export default {
    name: "Classes",

    data() {
        return {
            ClassElement: ClassList,
        };
    },
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";
img {
    max-width: 100%;
    height: 100%;
}
li {
    color: white;
    font-size: 0.9rem;
    .grey {
        color: #c5c3de;
    }
}
.title {
    color: $secondary;
    font-weight: 300;
}
.description {
    color: $text-grey;
}
.left {
    background-color: $secondary;
}
.box-border {
    border-right: 1px solid #c5c3de;
    padding-right: 15px;
}
.right {
    position: relative;
    div:first-child {
        font-size: .8rem;
        padding: 5px 5px 5px 10px;
        background-color: $main;
        color: white;
        text-transform: uppercase;
        width: 50%;
        height: 40px;
        position: absolute;
        right: 0;
        bottom: 0;
        img {
            width: 20px;
        }
    }
}
</style>
