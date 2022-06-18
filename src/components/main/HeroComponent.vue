<template>
    <div class="container" style="pt-15">
        <div class="row">
            <div class="col" lg="6">
                <h2 class="intro-text">Welcome to ImTraveler</h2>
                <p class="description">Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                    Fuga, aperiam ipsum eveniet ipsam eligendi doloribus voluptatum beatae neque cum,
                    laudantium facilis, autem dicta nulla libero quas in sunt quibusdam animi!</p>
                <button class="btn btn-success" rounded> Get Started </button>
                <button class="btn btn text-white" style="background-color: indigo" rounded> Watch Video </button>

            </div>
            <div class="col" lg="6">
                <img src="./../../assets/hero-img.jpg" alt="hero-img" style="width:100%">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "HeroComponent",

}
</script>

<style>
h2.intro-text {
    font-size: 60px;
    font-weight: bold;
    font-family: sans-serif;
    color: #444
}
p.description {
    font-size: 19px;
    font-family: sans-serif;
    margin: 32px 0px;
    color: #444444
}
</style>