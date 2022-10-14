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
        <img
          src="https://images.unsplash.com/photo-1487058792275-0ad4aaf24ca7?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80"
          alt="project1"
        />
        <h3 class="projectName">AI project</h3>
        <p class="desc">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Autem,
          laudantium.
        </p>
        <a href="#" class="projectLink">See project</a>
      </div>
      <div class="project">
        <img
          src="https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=774&q=80"
          alt="project1"
        />
        <h3 class="projectName">Python project</h3>
        <p class="desc">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Autem,
          laudantium.
        </p>
        <a href="#" class="projectLink">See project</a>
      </div>
      <div class="project">
        <img
          src="https://images.unsplash.com/photo-1531297484001-80022131f5a1?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=820&q=80"
          alt="project1"
        />
        <h3 class="projectName">Javascript project</h3>
        <p class="desc">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Autem,
          laudantium.
        </p>
        <a href="#" class="projectLink">See project</a>
      </div>
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
  background: black;
  /* background-color: #b29e9c; */
  background-position: center center;
  background-attachment: fixed;
  background-repeat: no-repeat;
  /* background-size: contain; */
  @apply flex flex-col  font-customOne text-white;
}
.headerSection {
  @apply mx-auto pt-5 capitalize mt-10 font-comfortaa text-xl;
}
.headerSection span {
  @apply text-4xl capitalize font-silkscreen;
}
img {
  @apply w-44 object-contain rounded shadow-xl;
}
#about {
  /* backdrop-filter: blur(2px); */
  @apply flex flex-col items-center justify-start text-left pt-14 px-20 mt-5;
}
#about h2,
#projects h2 {
  @apply text-3xl mb-4 font-silkscreen uppercase tracking-widest;
}
#about p {
  @apply p-5 rounded-md shadow-md mb-5 font-extralight bg-gradient-to-bl from-black via-gray-900 to-black font-overpass mx-32 py-10;
}
#projects {
  /* backdrop-filter: blur(2px); */
  @apply grid grid-cols-2 mt-5;
}
#projects h2 {
  @apply col-span-2 text-center mt-8;
}
#projects .project {
  @apply shadow-md mb-6 rounded-md p-8 w-3/4 mx-auto bg-gradient-to-br from-black via-gray-900 to-black;
}
.projectName {
  @apply font-bold text-2xl tracking-wider my-4 font-overpass uppercase border-b pb-2 mr-24 mb-8;
}
.project p {
  @apply my-5 text-xs font-extralight font-comfortaa;
}
#projects a {
  @apply bg-black text-white text-sm px-2 py-3 rounded shadow-xl uppercase font-silkscreen mt-4;
}
</style>
