<template>
    <section>
        <div class="container py-5">
            <div class="row justify-content-center mx-2s">
                <div class="col-2">
                    <h5>About Us</h5>
                    <p>Elipsis magna a nulla elite forte maecenas est elementum magna etos interdum movum morbi vehicula morbi. </p>
                    <img class="logo" src="../assets/images/logo_footer.png" alt="">
                </div>
                <div class="col-3 px-4">
                    <h5>Archives</h5>
                    <div class="month">October 2014 (2)</div>
                    <div class="month">September 2014 (2)</div>
                    <div class="month">August 2014 (2)</div>
                    <div class="month">July 2014 (2)</div>
                    <div class="month">June 2014 (2)</div>
                    <div class="month">May 2014 (1)</div>
                </div>
                <div class="col-3 px-4">
                    <h5>Our Features</h5>
                    <p>Nunc gravida rutrum mauris vehin hasellus ac pretium augue vivamul lacus ligul mattis ac vene: </p>
                    <ul class="list-unstyled">
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_4_alt.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Friendly and welcoming place
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_4_alt.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Science and art classes
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_4_alt.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Positive learning environment
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_4_alt.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Educational field trips
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_4_alt.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Writing and reading classes
                            </div>
                        </li>
                        <li class="d-flex align-items-center my-2">
                            <img
                                src="../assets/images/style_4_alt.png"
                                alt="check"
                            />
                            <div class="ms-2">
                                Science and art classes
                            </div>
                        </li>
                    </ul>
                </div>
                <div class="col-3 px-4">
                    <h5>Recent Post</h5>
                    <div class="d-flex justify-content-center align-items-center">
                        <div
                            class="img-container d-flex justify-content-center align-items-center"
                        >
                            <img src="../assets/images/blog_09-150x150.jpg" alt="clock" />
                        </div>
                        <div>
                            <h6>Drawing and Painting Lessons</h6>
                            <span> <img src="../assets/images/date_footer.png" alt=""></span>
                            <span>October 03, 2014</span>
                        </div>
                    </div>

                    <div class="d-flex justify-content-center align-items-center">
                        <div
                            class="img-container d-flex justify-content-center align-items-center"
                        >
                            <img src="../assets/images/blog_10-150x150.jpg" alt="clock" />
                        </div>
                        <div>
                            <h6>Fall Parents Meeting Day</h6>
                            <span> <img src="../assets/images/date_footer.png" alt=""></span>
                            <span>October 03, 2014</span>

                        </div>
                    </div>

                    <div class="d-flex justify-content-center align-items-center">
                        <div
                            class="img-container d-flex justify-content-center align-items-center"
                        >
                            <img src="../assets/images/blog_08-150x150.jpg" alt="clock" />
                        </div>
                        <div>
                            <h6>Birthday in Kindergarten</h6>
                            <span> <img src="../assets/images/date_footer.png" alt=""></span>
                            <span>september 20, 2014</span>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
name: 'Footer'
}
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";
section{
     background-image: url('../assets/images/pattern.png');
     color: $footer-color;
}
.logo{
    max-width: 100%;
}
p, li, span{
    font-size: .8rem;
    font-weight: 500;
}

h5{
    color: white;
    text-transform: uppercase;
    margin-bottom: 30px;
}

h6{
    color: white;
}

.month{
    border: .8px solid $footer-color;
    font-weight: 600;
    font-size: .7rem;
    text-transform: uppercase;
    padding: 10px;
    width: 100%;
    margin-bottom: 8px;
}

.img-container {
    margin-right: 15px;
    margin-bottom: 15px;
    img {
        width: 80px;
        height: 80px;
    }
}
div:last-child span{
    margin-right: 10px;
}

</style>