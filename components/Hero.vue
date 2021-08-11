<template>
  <div
    class="px-4 py-16 mx-auto sm:max-w-xl md:max-w-full lg:max-w-screen-xl md:px-24 lg:px-8 lg:py-20"
  >
    <div class="grid gap-5 row-gap-8 lg:grid-cols-2">
      <div class="flex flex-col justify-center">
        <div class="max-w-xl mb-6">
          <h2
            class="max-w-lg mb-6 font-sans text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl sm:leading-none"
          >
            Hi, my name is<br class="hidden md:block" />
            <span class="relative px-1">
              <div
                class="absolute inset-x-0 bottom-0 h-3 transform -skew-x-12 bg-teal-accent-400"
              ></div>
              <span class="relative inline-block text-deep-purple-accent-400"
                >Amirah Syamila</span
              >
            </span>
          </h2>
          <p class="text-base text-gray-700 md:text-lg">
            A Chemist with research experience in industrial and
            academic labs. Trained in varying research topics, including
            functional coatings, small molecule synthesis and catalysis.
          </p>
        </div>
      </div>
      <div>
        <img
          class="object-cover w-full h-56 rounded shadow-lg sm:h-96"
          src="~assets/img/portrait.jpg"
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.block-enter {
  opacity: 0;
}
.block-enter-active {
  transition: opacity 2s;
}
.block-leave-active {
  transition: opacity 2s;
  opacity: 0;
}
</style>
