<template lang="pug">
  section
    Loader/

    Header/

    HeroSection/

    SocialLinks/

    WorkExperience/

    Education/

    //- !-- References/> --

    //- !-- Portfolio/> --

    Extras/

    //- !-- ContactForm/> --

    Footer/

    //- !--====== Javascripts & Jquery ======--
    script(src="js/jquery-2.1.4.min.js")
    script(src="js/bootstrap.min.js")
    script(src="js/circle-progress.min.js")
    script(src="js/main.js")
</template>

<script>
import ContactForm from "~/components/ContactForm.vue";
import Education from "~/components/Education.vue";
import Extras from "~/components/Extras.vue";
import Footer from "~/components/Footer.vue";
import Header from "~/components/Header.vue";
import HeroSection from "~/components/HeroSection.vue";
import Loader from "~/components/Loader.vue";
import Portfolio from "~/components/Portfolio.vue";
import References from "~/components/References.vue";
import SocialLinks from "~/components/SocialLinks.vue";
import WorkExperience from "~/components/WorkExperience.vue";

export default {
  components: {
    ContactForm,
    Education,
    Extras,
    Footer,
    Header,
    HeroSection,
    Loader,
    Portfolio,
    References,
    SocialLinks,
    WorkExperience,
  },
  head() {
    return {
      title: "Елена Иванова",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Елена Иванова. Персональная страница",
        },
      ],
      link: [
        // <!-- Google Fonts -->
        {
          href:
            "https://fonts.googleapis.com/css?family=Josefin+Sans:400,400i,600,600i,700",
          rel: "stylesheet",
        },

        // <!-- Stylesheets -->
        { rel: "stylesheet", href: "css/bootstrap.min.css" },
        { rel: "stylesheet", href: "css/font-awesome.min.css" },
        { rel: "stylesheet", href: "css/flaticon.css" },
        { rel: "stylesheet", href: "css/owl.carousel.css" },
        { rel: "stylesheet", href: "css/magnific-popup.css" },
        { rel: "stylesheet", href: "css/style.css" },
      ],
    };
  },
};
</script>

<style>
</style>

