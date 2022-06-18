<template>
    <div class="container my-15">
        <div class="row" style="justify-center">
            <div class="col" lg="12" style="text-center">
                <header class="text-h4" style="justify-center"> Project </header>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                    Fuga, aperiam ipsum eveniet ipsam eligendi doloribus voluptatum beatae neque cum,
                    laudantium facilis, autem dicta nulla libero quas in sunt quibusdam animi!</p>
            </div>
            <div class="col" lg="4" v-for="project in 3" :key="project">
                <div class="card mx-auto my-12" style="max-width:374px">
                    <img src="./../../assets/web/2.jpg" style="height:250px">
                    <div class="card-title">Web Developement</div>
                    <div class="card-text">
                        <div>Small plates, salads & sandwiches - an intimate setting with 12 indoor seats.</div>
                    </div>
                    <v-divider class="mx-4"></v-divider>
                    <div class="card-actions">
                        <button style="color:success" rounded>View Details</button>
                        <spacer/>
                        <rating :value="4.5" color="amber" dense half-increments readonly size="14"></rating>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Project',

}
</script>

<style>

</style>