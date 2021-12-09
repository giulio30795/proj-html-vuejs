<template>
    <div>
        <Bar
        :MainText="mainText1"
        :ButtonText="Button1"
        />
        <Divider 
        :Title="Title1"
        :Subtitle="Subtitle1"/>
        

    </div>
</template>

<script>
import Bar from './Bar.vue'
import Divider from './Divider.vue'
export default {
name: 'Maincontent',

components:{
    Bar,
    Divider,
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