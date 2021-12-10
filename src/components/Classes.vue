<template>
    <section class="container">
        <div class="row justify-content-center">
            <div class="col-4">
                <h3 class="title">
                    We provided four classes with nine to twenty children each aged twelve month to five years of age.
                </h3>
            </div>
            <div class="col-4">
                <p class="description">
                    Praesent arcu gravida vehicula est node maecenas loareet morbi a dosis luctus. Urna eget lacinia eleifend praesent luctus a arcu quis facilisis venenatis. Aenean interdum, nibh vitae sodales, magna ante feugiat elit maecenas.
                </p>
            </div>

            <ul class="row justify-content-center">
                <li v-for="(element, index) in ClassList" :key="`class-${index}`"
                class="col-4">
                    <div>
                        <h4>{{element.title}}</h4>
                        <div>{{element.subtitle}}</div>
                        <div>
                            <div>
                                <div>
                                    {{element.age}}
                                </div>
                                <div>{{element.old}}

                                </div>
                            </div>
                            <div>
                                <div>
                                    {{element.class_size}}
                                </div>
                                <div>
                                    {{element.class}}
                                </div>
                            </div>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
import ClassList from '@/DevData/ClassList.js'
export default {
name:'Classes',

ClassList: ClassList,

}
</script>

<style scoped lang="scss">
@import "@/style/variables.scss";

.title{
    color: $secondary;
    font-weight: 300;
}
.description{
    color: $text-grey;
}

</style>