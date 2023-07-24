<template>
  <div class="hero">
    <Navigation />
    <Header />
  </div>
  <div class="zero">
<Caraousel/>
<Services/>
  </div>
</template>

<script setup>
import Caraousel from "~/components/Caraousel.vue";
import Navigation from "~/components/Navigation.vue";
import Header from "~/components/Header.vue";
import Services from "~/components/Services.vue";
</script>

<style>
.hero{
 background-color: #F4F5F7;
}

.zero{
  background-color: #FCFCFC;
}
</style>
