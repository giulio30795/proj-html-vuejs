<template>
    <section>
        <div class="container py-5 d-flex justify-content-center">
            <div class="col-4">
                <span class="overview me-3">Overview</span>
                <span class="mission">Our Mission</span>
                <h3 class="my-4">
                    Our philosophy is learning through play as we offer a
                    stimulating environment for children.
                </h3>

                <div class="d-flex justify-content-center align-items-center">
                    <div
                        class="img-container d-flex justify-content-center align-items-center"
                    >
                        <img src="../assets/images/clock_alt.png" alt="clock" />
                    </div>
                    <div>
                        <h5>Full Day Sessions</h5>
                        <p>
                            Pulvinar est metro ligula blandit maecenas retrum
                            gravida cuprum. Maecenas node estibulum.
                        </p>
                    </div>
                </div>
                <div class="d-flex justify-content-center align-items-center">
                    <div
                        class="img-container d-flex justify-content-center align-items-center"
                    >
                        <img
                            src="../assets/images/diagram_alt.png"
                            alt="diagram"
                        />
                    </div>
                    <div>
                        <h5>Varied Class</h5>
                        <p>
                            Pulvinar est metro ligula blandit maecenas retrum
                            gravida cuprum. Maecenas node estibulum.
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-4">
                <div class="big-image">
                    <img src="../assets/images/gallery_01.jpg" alt="Bambini" />
                    <div class="slider-right">
                        <img src="../assets/images/slider_next.png" alt="" />
                    </div>
                    <div class="slider-left">
                        <img
                            src="../assets/images/slider_previous.png"
                            alt=""
                        />
                    </div>
                </div>
                <div class="small-image d-flex justify-content-between">
                    <img
                        src="../assets/images/gallery_07-690x506.jpg"
                        alt="Bambini"
                    />
                    <img src="../assets/images/gallery_01.jpg" alt="Bambini" />
                    <img
                        src="../assets/images/gallery_08-690x506.jpg"
                        alt="Bambini"
                    />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "OurMission",
};
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

section {
    background-color: $background-grey;
}
.overview,
.mission {
    padding: 10px 15px;
    font-size: 1.2rem;
    font-weight: 300;
}
.overview {
    background-color: $main;
    color: white;
}

.mission {
    color: $text-grey;
    border-bottom: 1px solid #e8e8e8;
}
h3 {
    color: $secondary;
    font-weight: 300;
}

.img-container {
    margin-right: 30px;
    background-color: $main;
    width: 60px;
    height: 60px;
    border-radius: 50px;
    flex-shrink: 0;
    img {
        width: 30px;
        height: 30px;
    }
}

h5 {
    color: $secondary;
    font-weight: 200;
}
p {
    color: $text-grey;
}

.big-image {
    margin-left: 20px;
    position: relative;
    img {
        max-width: 100%;
    }
}

.slider-right,
.slider-left {
    width: 40px;
    height: 40px;
    background-color: $main;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
}

.slider-left {
    left: 0;
}
.slider-right {
    right: 0;
}

.small-image {
    margin-left: 20px;
    margin-top: 10px;
    img {
        padding-bottom: 10px;
        max-width: 32%;
    }
}
.small-image img:nth-child(2) {
    border-bottom: 2px solid $main;
}
</style>
