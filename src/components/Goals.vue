<template>
    <section class="py-5">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-4">
                    <h3>
                        We have been educating children for over fifteen years.
                        Our goal is to create a place that engages each child.
                    </h3>
                    <p>
                        Praesent arcu gravida vehicula est node maecenas loareet
                        morbi a dosis luctus. Urna eget lacinia eleifend
                        praesent luctus a arcu quis facilisis venenatis aenean
                        interdum.
                    </p>
                    <ul class="list-unstyled">
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_1.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Comprehensive reporting on individual
                                achievement
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_1.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Educational field trips and school presentations
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_1.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Individual attention in a small-class setting
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_1.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Learning program with after-school care
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_1.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Opportunities to carry out scientific
                                investigations
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_1.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Positive learning environment for your child
                            </div>
                        </li>
                    </ul>
                </div>
                <div class="col-4">
                    <ul class="d-flex justify-content-center flex-wrap">
                        <li
                            class="col-6 text-center d-flex flex-column justify-content-start align-items-center"
                            v-for="(element, index) in GoalsList"
                            :key="`welcome-${index}`"
                        >
                            <div
                                class="d-flex justify-content-center align-items-center circle"
                            >
                                <img
                                    :src="
                                        require(`../assets/images/${element.img}`)
                                    "
                                    alt="element.title"
                                />
                            </div>
                            <h4 class="my-3">{{ element.title }}</h4>
                            <p>{{ element.text }}</p>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import GoalsList from '@/DevData/GoalsList.js'
export default {
    name: "Goals",

    data(){
        return {
            GoalsList: GoalsList,
        }
    }
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

section {
    background-color: $background-grey;
}

h3, h4 {
    color: $secondary;
    font-weight: 300;
}
p,
li {
    color: $text-grey;
}

.circle{
    background-color: white;
    width:80px;
    height: 80px;
    border-radius: 40px;
    vertical-align: middle;
    img{
        width: 30px;
    }
}
</style>
