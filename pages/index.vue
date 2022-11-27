<template>
  <main>
    <div class="headerSection">
      <vue-typed-js
        :strings="['Designing', 'Developing', 'Deploying']"
        :loop="true"
        :typeSpeed="150"
        :startDelay="1200"
        :smartBackspace="true"
        :backSpeed="50"
      >
        <h1>
          <span class="typing"></span> <br />
          progressive web apps since 2019.
        </h1>
      </vue-typed-js>
    </div>
    <div id="about">
      <h2 class="aboutHeader">Who</h2>
      <p class="tracking-normal">
        Sapwavino Samari is a human being that designs, develops and deploys
        mobile-first user-friendly progressive web applications that make life
        easier for individuals and businesses with technologies like
        <span class="font-bold font-comfortaa tracking-wider"
          >Javascript, Python, Google Firebase, Vue js, & Amazon Web
          Services.</span
        >
      </p>
      <IconGroup />
    </div>
    <div id="projects">
      <h2>What</h2>
      <div class="project">
        <div class="grid grid-cols-2 place-items-center p-4 rounded-xl">
          <img
            src="https://i.postimg.cc/XqDYxPgx/smartmockups-l98y67y4.png"
            alt="project1"
          />
          <img
            src="https://i.postimg.cc/k448Tr5G/smartmockups-l9a3fn2p.png"
            class="h-28"
          />
        </div>
        <h3 class="projectName">Lumen Bar & Grill</h3>
        <h4>Location: 🇬🇭</h4>
        <h4>Platforms: 📱🖥️</h4>
        <p class="desc">
          A web app for placing and managing orders at Lumen Bar & Grill Eastern
          Region, Ghana. It comes with a fully managed admin panel, flutterwave
          payment gateway and realtime data storage for the menu using Firebase.
          <br />[Note:] This is not a demo. You will be charged for orders you
          make.
        </p>
        <a
          href="https://lumenbarandgrill.vercel.app"
          class="projectLink"
          target="_blank"
          >See project</a
        >
        <ul class="technologies">
          <li>Nuxt Js</li>
          <li>Google Firebase</li>
          <li>Flutterwave</li>
          <li>Tailwind CSS</li>
        </ul>
      </div>
      <div class="project">
        <div class="grid grid-cols-2 place-items-center p-4 rounded-xl">
          <img
            src="https://i.postimg.cc/L8bHbVX5/smartmockups-l9a0zg5o.png"
            alt="project1"
          />
          <img
            src="https://i.postimg.cc/cHst6p3T/smartmockups-l9a3d6oe.png"
            class="h-28"
          />
        </div>
        <h3 class="projectName">Serah Johnson</h3>
        <h4>Location: 🇳🇬🌍</h4>
        <h4>Platforms: 📱🖥️</h4>
        <p class="desc">
          Serah johnson is a professional voice actor and coach with years of
          experience in radio and voice acting. This web app was designed to
          enable her onboard new clients easily and showcase her work with a
          custom audio player and contact form. <br />
          [Note:] It works. Reach out to her for your projects.
        </p>
        <a
          href="https://serahjohnson.vercel.app"
          target="_blank"
          class="projectLink"
          >See project</a
        >
        <ul class="technologies">
          <li>Nuxt Js</li>
          <li>Google Firebase</li>
          <li>Flutterwave</li>
          <li>Tailwind CSS</li>
        </ul>
      </div>
    </div>
    <div id="skills">
      <h2>How</h2>
      <SkillsIcons />
    </div>
  </main>
</template>

<script>
import GlitchText from "~/components/GlitchText.vue";
export default {
  name: "IndexPage",
  components: { GlitchText },
};
</script>

<style scoped>
main {
  @apply flex flex-col  font-customOne text-white bg-black;
}
.headerSection {
  @apply mx-auto pt-20 md:pt-5 capitalize mt-10 font-comfortaa text-xl;
}
.headerSection span {
  @apply text-4xl capitalize font-silkscreen;
}
#about {
  @apply flex flex-col items-center justify-start text-left pt-14 md:px-20 md:mt-5 my-1 px-5;
}
#about h2,
#projects h2,
#skills h2 {
  @apply text-3xl md:mb-4 font-silkscreen uppercase tracking-widest;
}
#about p {
  @apply p-5 rounded-md shadow-md mb-5 font-extralight bg-gradient-to-bl from-black via-gray-900 to-black font-overpass md:mx-32 md:py-10 py-5 text-center md:text-left;
}
#projects {
  /* backdrop-filter: blur(2px); */
  @apply md:grid md:grid-cols-2 mt-5;
}
#projects h2 {
  @apply col-span-2 text-center mt-8;
}
#projects h4 {
  @apply text-sm;
}
#projects .project {
  @apply shadow-md mb-6 rounded-md p-8 md:w-3/4 mx-auto bg-gradient-to-br from-black via-gray-900 to-black text-center md:text-left w-5/6;
}
.projectName {
  @apply font-bold text-2xl tracking-wider my-4 font-overpass uppercase border-b pb-2 md:mr-24 md:mb-8;
}
.project p {
  @apply my-5 text-xs font-extralight font-comfortaa leading-5;
}
#projects a {
  @apply bg-black text-white text-sm px-2 py-3 rounded shadow-xl uppercase font-silkscreen mt-4;
}
#skills {
  @apply flex flex-col items-center justify-center my-5;
}
.technologies {
  @apply text-xs grid grid-cols-2 md:w-5/6 my-5 mx-auto;
}
.technologies li {
  @apply tracking-tight my-2 bg-gray-700 w-5/6 rounded-3xl py-1 text-center bg-opacity-30 text-gray-400 font-customOne;
}
</style>
