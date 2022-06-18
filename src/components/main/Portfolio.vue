<template>
  <div class="container" style="my-15">
        <div class="row" style="justify-center">
            <div class="col" lg="12" style="text-center">
                <header style="text-h4; justify-center;"> Portfolio </header>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                    Fuga, aperiam ipsum eveniet ipsam eligendi doloribus voluptatum beatae neque cum,
                    laudantium facilis, autem dicta nulla libero quas in sunt quibusdam animi!</p>
            </div>
            <div class="col" lg="12">
                <div style="text-center">
                    <button @click="activeResult = 'webapp'"  :color="activeResult === 'webapp' ? 'success' : ''" class="mx-5"> Web App </button>
                    <button @click="activeResult = 'mobileapp'" :color="activeResult === 'mobileapp' ? 'success' : ''" class="mx-5"> Mobile App </button>
                    <button @click="activeResult = 'desktopapp'" :color="activeResult === 'desktopapp' ? 'success' : ''" class="mx-5"> Desktop App </button>
                </div>
            </div>
            <slot v-if="activeResult === 'webapp'">
                <div class="col" lg="3" v-for="(web, webindex) in webApps" :key="webindex">
                    <div class="card">
                        <img :src="web.image" class="white--text align-end" style="gradient:to bottom; rgba(0, 0, 0,.1); rgba(0, 0, 0,.5); height:200px;">
                            <div class="card-title">{{ web.title }}</div>                        
                    </div>
                </div>
            </slot>
            <slot v-if="activeResult === 'mobileapp'">
                <div class="col" lg="3" v-for="(mobile, mobileindex) in mobileApps" :key="mobileindex">
                    <div class="card">
                        <img :src="mobile.image" class="white--text align-end" style="gradient:to bottom; rgba(0, 0, 0,.1); rgba(0, 0, 0,.5); height:200px;">
                            <div class="card-title">{{ mobile.title }}</div>                        
                    </div>
                </div>
            </slot>
        </div>
    </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Portfolio',

    data() {
        return {
            activeResult: 'webapp',
            webApps: [
                {title: 'Great mountain', image: 'https://www.iucn.org/sites/dev/files/styles/850x500_no_menu_article/public/content/images/2020/shutterstock_1458128810.jpg?itok=sKSJDbYv'},
                {title: 'Chicago Illinois', image: 'https://images.pexels.com/photos/161963/chicago-illinois-skyline-skyscrapers-161963.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2'},
                {title: 'Japan street', image: 'https://images.unsplash.com/photo-1542052125323-e69ad37a47c2?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80'},
                {title: 'Chicago', image: 'https://imgs-akamai.mnstatic.com/ab/a3/aba352133ce3432ccc4295d77e9ac860.jpg'},
                {title: 'Chicago', image: 'https://images8.alphacoders.com/813/thumb-1920-813547.jpg'},
                {title: 'Japan street', image: 'https://images.unsplash.com/photo-1540959733332-eab4deabeeaf?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80'},
                {title: 'Chicago', image: 'https://c4.wallpaperflare.com/wallpaper/510/963/728/5bd16fa7a92e9-wallpaper-preview.jpg'},
                {title: 'Japan street', image: 'https://images.unsplash.com/photo-1534359076531-3b7af836d7f2?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1yZWxhdGVkfDJ8fHxlbnwwfHx8fA%3D%3D&w=1000&q=80'}
            ],
            mobileApps: [
                {title: 'Great mountain', image: 'https://www.iucn.org/sites/dev/files/styles/850x500_no_menu_article/public/content/images/2020/shutterstock_1458128810.jpg?itok=sKSJDbYv'},
                {title: 'Chicago Illinois', image: 'https://images.pexels.com/photos/161963/chicago-illinois-skyline-skyscrapers-161963.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2'},
                {title: 'Japan street', image: 'https://images.unsplash.com/photo-1542052125323-e69ad37a47c2?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80'},
                {title: 'Chicago', image: 'https://imgs-akamai.mnstatic.com/ab/a3/aba352133ce3432ccc4295d77e9ac860.jpg'},
                {title: 'Chicago', image: 'https://images8.alphacoders.com/813/thumb-1920-813547.jpg'}
            ]
        }
    }
}
</script>

<style>

</style>