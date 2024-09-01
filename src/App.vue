


<template>
  <div>
    <div class="container">
      <header class="d-flex justify-content-center py-3">
        <ul class="nav nav-pills">
          <li class="nav-item ">
            <RouterLink to="/" class="nav-link fw-bold">Home</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink to="/About" class="nav-link fw-bold">About</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink :to="{name:'Projects'}" class="nav-link fw-bold">Projects</RouterLink>
          </li>
        </ul>
      </header>
    </div>
  </div>


  <!-- <RouterView /> -->
  <HomeView style="height: 10%;"></HomeView>
  <AboutView></AboutView>
  <ProjectsView></ProjectsView>
</template>

<style>

.router-link-active{
  background-color: aquamarine;
  border-bottom:.25rem solid transparent;
  color:rgba(red, green, blue);
}
.fw-bold{
  font-weight: 700!important; 
}
</style>


<script >
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import HomeView from "./views/HomeView.vue";
import AboutView from "./views/AboutView.vue";
import ProjectsView from "./views/ProjectsView.vue";


export default {
  components:{HomeView,AboutView,ProjectsView},
  data() {
    return {};
  },
  mounted(){},


  methods:{}

};
</script>



<!-- <template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>


<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
-->