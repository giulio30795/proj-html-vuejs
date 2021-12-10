<template>
    <div>
        <Bar
        :MainText="mainText1"
        :ButtonText="Button1"
        />
        <Divider 
        :Title="Title1"
        :Subtitle="Subtitle1"/>
        <WelcomePart />
        <OurMission />

    </div>
</template>

<script>
import Bar from './Bar.vue'
import Divider from './Divider.vue'
import WelcomePart from './WelcomePart.vue'
import OurMission from './OurMission.vue'
export default {
name: 'Maincontent',

components:{
    Bar,
    Divider,
    WelcomePart,
    OurMission,
},

data() {
    return {
        mainText1: 'How To Enroll Your child to a Class?',
        Button1: 'Learn More',
        Title1: 'Welcome to Fable',
        Subtitle1: 'Fable daycare, preschool, and kindergarten',
    }
},

}
</script>

<style>

</style>