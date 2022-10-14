<template>
  <nav>
    <GlitchText :text="`Sapwavino`" class="GlitchText" />
    <nuxt-link to="/#about">Who</nuxt-link>
    <nuxt-link to="/#projects">What</nuxt-link>
    <nuxt-link to="/#skills">How</nuxt-link>
    <nuxt-link to="/#contact">Where</nuxt-link>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
nav {
  @apply md:flex items-center justify-between shadow-md fixed w-full z-50 top-0 font-silkscreen text-white bg-black bg-opacity-80 grid grid-cols-2;
}
.GlitchText {
  @apply col-span-2;
}
a {
  -webkit-backdrop-filter: blur(22px);
  backdrop-filter: blur(22px);
  border: 1px solid rgba(255, 255, 255, 0.229);
  @apply font-medium  hover:bg-gray-900 hover:text-gray-200 transform transition-all duration-300 ease-in-out mx-auto px-8 py-2 hover:shadow-2xl shadow-md rounded-md tracking-wider text-sm hover:scale-125 border-r-0 border-l-0;
}
</style>
