<template>
  <div class="home">
    <app-header />
    <app-intro />
    <app-skills />
    <app-experience />
    <app-education />
    <app-portfolio />
    <app-footer />
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader.vue";
import AppIntro from "@/components/AppIntro.vue";
import AppSkills from "@/components/AppSkills.vue";
import AppExperience from "@/components/AppExperience.vue";
import AppEducation from "@/components/AppEducation.vue";
import AppPortfolio from "@/components/AppPortfolio.vue";
import AppFooter from "@/components/AppFooter.vue";

export default {
  name: "HomeView",
  components: {
    AppHeader,
    AppIntro,
    AppSkills,
    AppExperience,
    AppEducation,
    AppPortfolio,
    AppFooter,
  },
  data(){
    return{

    }
  },
  mounted(){
    document.querySelectorAll(".start-move").forEach((el, indx) => {
      setTimeout(() => {
        el.classList.add("move");
      }, 1000 + indx * 200);
    });

  }
};
</script>

<style lang="scss" scoped>




</style>
