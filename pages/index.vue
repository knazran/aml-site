<template>
  <div class="">
    <hero></hero>
    <project-section></project-section>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Hero from '~/components/Hero.vue'
import ProjectSection from '~/components/ProjectSection.vue'
import Subheader from '~/components/Subheader'

export default {
  transition: {
    name: 'home',
    mode: 'out-in',
  },
  components: {
    Logo,
    Hero,
    ProjectSection,
    Subheader,
  },
  head() {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' },
      ],
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Khairul Nazran (Knazran) personal site and blog',
        },
        {
          name: 'og:image',
          content: 'https://www.mugshotbot.com/m?url=https://www.knazran.dev',
        },
      ],
    }
  },
}
</script>

<styles>
  .home-enter-active, .home-leave-active { transition: opacity .5s; }
  .home-enter, .home-leave-active { opacity: 0; }
</styles>
