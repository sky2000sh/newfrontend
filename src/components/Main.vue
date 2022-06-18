<template>
    <Header/>

    <HeroComponent/>
    <AboutUs/>
    <Portfolio/>
    <Project/>



    

    
</template>

<script>
import header from './Header.vue'
import heroComponent from './main/HeroComponent.vue'
import aboutUs from './main/AboutUs.vue'
import portfolio from './main/Portfolio.vue'
import project from './main/Project.vue'

export default {
    name: 'App',

    components: {
        Header: header,
        HeroComponent: heroComponent,
        AboutUs: aboutUs,
        Portfolio: portfolio,
        Project: project,
    },

    data() {
        return {
            menus: [
            {title: 'Home', route: 'home'},
            ]
            
            
        }
    }
}
</script>