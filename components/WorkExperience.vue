<template>
  <ResumeSection :title="title" :items="items" />
</template>

<script>
import ResumeSection from "~/components/ResumeSection.vue";

export default {
  components: {
    ResumeSection,
  },
  data() {
    return {
      title: "Опыт работы",
      items: [
        {
          period: "2016-Настоящее время",
          workplace: "Частный агент",
          occupation: "",
          description:
            "Куплю и продам то, что никто не сможет",
        },
      ],
    };
  },
};
</script>
