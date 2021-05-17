<template>
  <div class="center examplex">
    <vs-navbar
      center-collapsed
      v-model="active"
      id="header"
      text-white
      color="#072b43">
      <vs-navbar-item :active="active === 'guide'" to id="guide">
        Accueil
      </vs-navbar-item>
      <vs-navbar-item :active="active === 'docs'" id="docs">
        Présentation
      </vs-navbar-item>
      <vs-navbar-item :active="active === 'components'" id="components">
        Projet Professionnel
      </vs-navbar-item>
      <vs-navbar-item :active="active === 'license'" id="license">
        Portfolio
      </vs-navbar-item>
    </vs-navbar>
  </div>
</template>

<script>
    export default {
        name: "Header",
        data:() => ({
          active: 'guide'
        })
    }
</script>

<style scoped>
#header{
  height: 5%;
  font-family: Roboto, sans-serif;
}
</style>
