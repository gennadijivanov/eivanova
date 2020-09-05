<template>
  <ResumeSection :title="title" :items="items" withBackground />
</template>

<script>
import ResumeSection from "~/components/ResumeSection.vue";

export default {
  components: {
    ResumeSection,
  },
  data() {
    return {
      title: "Образование",
      items: [
        {
          period: "1999-2004",
          workplace: "Тульский Государственный Университет",
          occupation: "магистр",
          description:
            "Владыка электрохимии",
        },
      ],
    };
  },
};
</script>
