<template>
  <transition name="home">
    <div class="projectsWrap">
      <div class="projects">
        <Project
          title="Inverse"
          tools="Nextjs, Typescript, Redux, Cypress, Etherjs."
          about="Inverse allows creators to easily launch a digital collectible."
          site="https://www.inverse.wtf/"
        />
        <Project
          title="Abacus (Mobile and web)."
          tools="React native, Nextjs, Typescript, Cypress, RTK query, Redux. "
          about="Abacus helps users better manage  money by unifying banking, investment and crypto accounts into a single, secure app."
          site="https://www.trustabacus.com/"
        />
        <Project
          title="Rise."
          tools="React native, React-query, Typescript. "
          about="Simple assets investment app built with React native."
          site="https://www.trustabacus.com/"
          frontendrepo="https://github.com/Makinde1034/risevest-assessment"
        />
        <Project
          title="Qshop"
          tools="Nextjs, Typescript, React-Redux, Tailwindcss,"
          about="E-commerce platform."
          site="https://qshopp.vercel.app/"
          frontendrepo="https://github.com/Makinde1034/Qshop"
        />
        <Project
          title="Bookly"
          tools="VueJs, VueX, scss, "
          about="Event booking app"
          site="https://makinde-glover-task.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Glover-takehome-test"
        />
        <Project
          title="Photohome"
          tools="VueJs, VueX, scss,"
          about="Web app that gets beautiful images from unsplash"
          site="https://photohome.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Photo-home"
        />

        <Project
          title="Bejamas-shopping task"
          tools="Reactjs"
          about="Bejams frontend engineer task."
          site="https://bejamas-shopping.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Bejamas"
        />
        <Project
          title="Typing app"
          tools="Reactjs, Typescript"
          about="Typing test app. Calculates typing speed and accuracy."
          site="https://typing-testt.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Typing-test"
        />
      </div>
    </div>
  </transition>
</template>

<script>
export default {
  transition: 'home',
  head: {
    title: 'Projects',
    meta: [
      {
        hid: 'Makinde Tolu projects',
        name: 'Project',
        content: 'Makinde Tolu projects',
      },
    ],
  },
}
</script>

<style>
.projectsWrap {
  padding: 100px 200px 100px 200px;
}

.projects {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  gap: 30px;
  color: white;
}

.projects div {
  border: 1px solid white;
  border-radius: 5px;
}


/* transition classes */

.home-enter-active {
  transition: all 0.3s ease;
  opacity: 1;
  /* transform: translateY(0px); */
  /* transform: scale(1); */
}

.home-enter {
  opacity: 0;
  /* transform: translateY(50px); */
  /* transform: scale(0.5); */
}

.home-leave-active {
  opacity: 0;
  /* transform: translateY(50px); */
  transition: all 0.3s ease;
  /* transform: scale(0.5); */
}

.home-leave {
  opacity: 1;
  /* transform: translateY(50px); */
  /* transform: scale(0.5); */
}

@media screen and (max-width: 480px) {
  .projectsWrap {
    padding: 50px 20px 0px 20px;
  }

  .projects {
    grid-template-columns: 1fr;
  }
}

@media screen and (min-width: 480px) and (max-width: 768px) {
  .projectsWrap {
    padding: 50px 20px 0px 20px;
  }

  .projects {
    grid-template-columns: 1fr 1fr;
  }
}

@media screen and (min-width: 768px) and (max-width: 1024px) {
  .projectsWrap {
    padding: 50px 20px 0px 20px;
  }

  .projects {
    grid-template-columns: 1fr 1fr 1fr;
  }
}
</style>
