<template>
  <div class="home">
    <app-header> </app-header>
    <app-intro> </app-intro>
    <app-skills> </app-skills>
    <app-experience> </app-experience>
    <app-education> </app-education>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader.vue";
import AppIntro from "@/components/AppIntro.vue";
import AppSkills from "@/components/AppSkills.vue";
import AppExperience from "@/components/AppExperience.vue";
import AppEducation from "@/components/AppEducation.vue";

export default {
  name: "Home",
  components: {
    AppHeader,
    AppIntro,
    AppSkills,
    AppExperience,
    AppEducation,
  },
};
</script>
