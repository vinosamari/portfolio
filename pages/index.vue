<template>
  <main>
    <div class="headerSection">
      <vue-typed-js
        :strings="['Designing', 'Developing', 'Deploying']"
        :loop="true"
        :typeSpeed="150"
        :startDelay="2000"
        :smartBackspace="true"
        :loopCount="4"
      >
        <h1>
          <span class="typing"></span> <br />
          progressive web apps since 2019.
        </h1>
      </vue-typed-js>
    </div>
    <div id="about">
      <h2 class="aboutHeader">Who?</h2>
      <p class="aboutSummaru">
        I'm a human being that designs web applications that make life easier
        for individuals and businesses by using technologies like
        <span class="font-bold"
          >Javascript, Python, Google Firebase, Vue/Nuxt js, & Amazon Web
          Services</span
        >, to develop mobile-first user-friendly progressive web applications.
      </p>
    </div>
    <div id="projects">
      <h2>What?</h2>
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
  @apply flex flex-col items-center font-customOne text-white;
}
.headerSection {
  @apply text-center mx-auto pt-5 capitalize mt-10;
}
.headerSection span {
  @apply text-3xl capitalize font-mono;
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
  @apply text-3xl font-bold mb-4 uppercase underline;
}
#about p {
  background: rgba(254, 252, 251, 0.102);
  -webkit-backdrop-filter: blur(22px);
  backdrop-filter: blur(22px);
  border: 1px solid rgba(235, 210, 204, 0.1);
  @apply p-5 rounded-sm shadow-md mb-5 font-extralight text-lg;
}
#projects {
  /* backdrop-filter: blur(2px); */
  @apply grid grid-cols-2;
}
#projects h2 {
  @apply col-span-2 text-center mt-8;
}
#projects .project {
  background: rgba(255, 255, 255, 0.131);
  -webkit-backdrop-filter: blur(22px);
  backdrop-filter: blur(22px);
  border: 1px solid rgba(235, 210, 204, 0.1);
  @apply shadow-md mb-6 rounded-md p-5 w-3/4 mx-auto;
}
.projectName {
  @apply font-bold text-2xl tracking-wider my-3;
}
.project p {
  @apply mb-5 text-xs font-extralight;
}
#projects a {
  @apply bg-black font-mono text-white text-sm px-2 py-3 rounded shadow-xl uppercase;
}
</style>
