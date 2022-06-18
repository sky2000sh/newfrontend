<template>
    <nav class="navbar bg-light">
      <div class="container-fluid">
        <span class="mainTitle">ImTraveler</span>

        <ul class="nav justify-content-end">

          <!-- <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Active</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link disabled">Disabled</a>
          </li> -->

          <li class="nav-item" @click="$router.push('/')">
            <a class="nav-link">Active</a>
          </li>
          <li class="nav-item" @click="$router.push('/about-us')">
            <a class="nav-link">About us</a>
          </li>
          <li class="nav-item" @click="$router.push('/portfolio')">
            <a class="nav-link">Portfolio</a>
          </li>
          <li class="nav-item" @click="$router.push('/project')">
            <a class="nav-link">Project</a>
          </li>
          <li class="nav-item" @click="$router.push('/gallery')">
            <a class="nav-link">Gallery</a>
          </li>
          <li class="nav-item" @click="$router.push('/contact')">
            <a class="nav-link">Contact</a>
          </li>

          <button type="button" class="btn btn-primary" @click="moveLogin">Get Started</button>
        </ul>

        
      </div>

      


    </nav>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Header',

    data() {
        return {
          
        }
    },

    methods: {
        moveLogin() {
            this.$router.push('/login')
        }
    },
}
</script>

<style>
.mainTitle {
    font-size: 32px;
    font-weight: bold;
    font-family: sans-serif;
    color: #4caf50
}

</style>