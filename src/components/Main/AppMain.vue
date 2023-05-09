<script>
import AppHero from "./AppHero.vue";
import ProjectsSection from "./ProjectsSection.vue";
import ContactSection from "./ContactSection.vue";
export default {
  name: "AppMain",
  components: {
    AppHero,
    ProjectsSection,
    ContactSection,
  },
};
</script>

<template>
  <main>
    <AppHero />
    <ProjectsSection />
    <ContactSection />
  </main>
</template>

<style lang="scss" scoped></style>
