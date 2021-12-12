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
        <Goals />
        <Bar
        :MainText="mainText2"
        :ButtonText="Button2" />
        <Divider 
        :Title="Title3"
        :Subtitle="Subtitle3"
        />
        <Staff />
        <FablePlace />

    </div>
</template>

<script>
import Bar from './Bar.vue'
import Divider from './Divider.vue'
import WelcomePart from './WelcomePart.vue'
import OurMission from './OurMission.vue'
import Numbers from './Numbers.vue'
import Classes from './Classes.vue'
import Goals from './Goals.vue'
import Staff from './Staff.vue'
import FablePlace from './FablePlace.vue'



export default {
name: 'Maincontent',

components:{
    Bar,
    Divider,
    WelcomePart,
    OurMission,
    Numbers,
    Classes,
    Goals,
    Staff,
    FablePlace,
},

data() {
    return {
        mainText1: 'How To Enroll Your child to a Class?',
        Button1: 'Learn More',
        Title1: 'Welcome to Fable',
        Subtitle1: 'Fable daycare, preschool, and kindergarten',
        Title2: 'Our Classes',
        Subtitle2: 'Our preschool program has four dedicated classes',
        mainText2: 'See Our Kindergarten Photo Gallery!',
        Button2: 'View Gallery',
        Title3: 'Meet Our Staff',
        Subtitle3: 'With education and experience in early childhood care',
    }
},

}
</script>

<style>

</style>