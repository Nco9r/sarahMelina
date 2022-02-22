<template>
  <main>
    <hero />
    <baseline/>
    <services-index/>
    <cta/>
    <projets/>
    <clients/>
    <blog-index/>
    <insta/>
  </main>
</template>

<script>
import Baseline from '../components/PageIndex/Baseline.vue'
import BlogIndex from '../components/PageIndex/BlogIndex.vue'
import Clients from '../components/PageIndex/Clients.vue'
import Cta from '../components/PageIndex/Cta.vue'
import Hero from '../components/PageIndex/Hero.vue'
import Insta from '../components/PageIndex/Insta.vue'
import Projets from '../components/PageIndex/Projets.vue'
import ServicesIndex from '../components/PageIndex/ServicesIndex.vue'
export default {
  components: { Hero, Baseline, ServicesIndex, Cta, Projets, Clients, BlogIndex, Insta },
}
    
</script>

<style scoped></style>
