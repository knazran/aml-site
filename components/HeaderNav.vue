<template>
  <div class="flex flex-col md:flex-row space-y-4 md:space-y-0 justify-between">
    <nuxt-link :to="`/`">
      <div class="text-center md:text-left">
        <h2 class="font-raleway tracking-wide font-black text-xl">AML</h2>
      </div>
    </nuxt-link>

    <div id="nav" class="flex justify-center lg:justify-start space-x-6 text-md">
      <!-- <nuxt-link
        class="text-primary-700 hover:text-primary-900 hover:font-semibold"
        :to="`/about`"
      >About</nuxt-link>
      <nuxt-link
        class="text-primary-700 hover:text-primary-900 hover:font-semibold"
        :to="`/project`"
      >Projects</nuxt-link>
      <nuxt-link
        class="text-primary-700 hover:text-primary-900 hover:font-semibold"
        :to="`/blog`"
      >Blog</nuxt-link> -->
    </div>
    <div id="nav" class="flex justify-center lg:justify-start space-x-6 text-sm">
      <a class="text-gray-700 hover:text-black" href="https://www.linkedin.com/in/amirah-syamila-mat-lani-6a0a23b6/">
        <IconifyIcon :icon="icons.linkedin" height="24" />
      </a>
      <!-- <a class="text-gray-700 hover:text-black" href="https://github.com/knazran">
        <IconifyIcon :icon="icons.github" height="24" />
      </a> -->
      <!-- <a class="text-gray-700 hover:text-black" href="https://twitter.com/khairulnazran">
        <IconifyIcon :icon="icons.twitter" height="24" />
      </a> -->
    </div>
  </div>
</template>

<script>
import IconifyIcon from '@iconify/vue'
import linkedinFilled from '@iconify/icons-ant-design/linkedin-filled'
import githubFilled from '@iconify/icons-ant-design/github-filled'
import twitterOutlined from '@iconify/icons-ant-design/twitter-outlined'

export default {
  components: {
    IconifyIcon,
  },
  data() {
    return {
      icons: {
        linkedin: linkedinFilled,
        github: githubFilled,
        twitter: twitterOutlined,
      },
    }
  },
}
</script>