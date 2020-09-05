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
      title: "Education",
      items: [
        {
          period: "1999-2004",
          workplace: "TulGU",
          occupation: "Student",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed porttitor orci ut sapien scelerisque viverra. Sed trist ique justo nec mauris efficitur, ut lacinia elit dapibus. In egestas elit in dap ibus laoreet. Duis magna libero, fermentum ut facilisis id, pulvinar eget tortor. Vestibulum pelle ntesque tincidunt lorem, vitae euismod felis porttitor sed.",
        },
      ],
    };
  },
};
</script>
