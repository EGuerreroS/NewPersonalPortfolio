<template>
  <q-page class="flex column mainBg">
    <div class="q-ma-none">
      <PrincipalComponent/>
    </div>
    <div class="q-ma-none">
      <PhraseComponent/>
    </div>
    <div class="q-ma-none">
      <FormationComponent/>
    </div>
    <div class="q-ma-none">
      <ProjectsComponent/>
    </div>
    <div class="q-ma-none">
      <FooterComponent/>
    </div>


  </q-page>
</template>

<script setup>
import PrincipalComponent from 'pages/PrincipalComponent.vue'
import PhraseComponent from 'pages/PhraseComponent.vue'
import FormationComponent from 'pages/FormationComponent.vue'
import ProjectsComponent from 'pages/ProjectsComponent.vue'
import FooterComponent from 'pages/FooterComponent.vue'


</script>
<style>
.mainBg {
  background: #060508;
  //background: radial-gradient(circle, rgba(43, 3, 84, 1) 0%, rgba(24, 3, 56, 1) 100%);
}
</style>
