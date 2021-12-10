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
        <Numbers />
        <Divider 
        :Title="Title2"
        :Subtitle="Subtitle2"/>
        <Classes />

    </div>
</template>

<script>
import Bar from './Bar.vue'
import Divider from './Divider.vue'
import WelcomePart from './WelcomePart.vue'
import OurMission from './OurMission.vue'
import Numbers from './Numbers.vue'
import Classes from './Classes.vue'

export default {
name: 'Maincontent',

components:{
    Bar,
    Divider,
    WelcomePart,
    OurMission,
    Numbers,
    Classes,
},

data() {
    return {
        mainText1: 'How To Enroll Your child to a Class?',
        Button1: 'Learn More',
        Title1: 'Welcome to Fable',
        Subtitle1: 'Fable daycare, preschool, and kindergarten',
        Title2: 'Our Classes',
        Subtitle2: 'Our preschool program has four dedicated classes'
    }
},

}
</script>

<style>

</style>