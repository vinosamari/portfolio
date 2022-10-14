<template>
  <nav>
    <GlitchText :text="`Sapwavino Samari`" />
    <nuxt-link to="/#about">About</nuxt-link>
    <nuxt-link to="/#skilss">Skills</nuxt-link>
    <nuxt-link to="/#projects">Projects</nuxt-link>
    <nuxt-link to="/#contact">Contact</nuxt-link>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
nav {
  /* backdrop-filter: blur(2px);
  background: rgb(93, 73, 84);
  background: linear-gradient(
    90deg,
    rgba(93, 73, 84, 1) 0%,
    rgba(121, 88, 97, 1) 35%,
    rgba(240, 222, 213, 1) 100%
  ); */
  @apply flex items-center justify-between shadow-md fixed w-full z-50 top-0 font-customOne text-white;
}
a {
  background: rgba(255, 255, 255, 0.2);
  -webkit-backdrop-filter: blur(22px);
  backdrop-filter: blur(22px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  @apply font-medium  hover:bg-customOne hover:text-white transform transition-all duration-500 ease-in-out mx-auto px-8 py-2 hover:shadow-2xl shadow-md rounded-sm tracking-wider text-sm underline;
}
</style>
