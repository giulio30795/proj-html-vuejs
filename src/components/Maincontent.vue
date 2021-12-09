<template>
    <div>
        <Bar
        :MainText="this.mainText1"
        :ButtonText="Button1"
        />

    </div>
</template>

<script>
import Bar from './Bar.vue'
export default {
name: 'Maincontent',

components:{
    Bar,
},

data() {
    return {
        mainText1: 'How To Enroll Your child to a Class?',
        Button1: 'Learn More'
    }
},

}
</script>

<style>

</style>