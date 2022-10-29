<template>
  <div class="home">
      <app-header> </app-header>
      <app-intro> </app-intro>
    </div>

</template>

<script>
import AppHeader from "@/components/AppHeader.vue";
import AppIntro from "@/components/AppIntro.vue";

export default {
  name: "Home",
  components: {
    AppHeader,
    AppIntro,
  },
};
</script>
