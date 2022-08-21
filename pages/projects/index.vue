<template>
  <transition name="home">
    <div class="projectsWrap">
      <div class="projects">
        <Project
          title="Transaction history"
          tools="Nextjs, Typescript, Nodejs, Graphql, Appollo client"
          about="Transaction list."
          site="https://makinde-helicarrier.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Helicarriers-task"
        />
        <Project
          title="Bosshall"
          tools="ReactJs(Typescript), Redux, NodeJs, SCSS, MongoDB"
          about="Video Sharing platform"
          frontendrepo="https://github.com/Makinde1034/Bosshall-frontend"
          backendrepo="https://github.com/Makinde1034/bosshall-backend"
          site="https://bosshall.netlify.app/"
        />
        <Project
          title="Naijchat"
          tools="ReactJs, NodeJs MongoDB, Socket io"
          about="Microblogging platform"
          site="https://naij.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/naij"
        />
        <Project
          title="Qshop"
          tools="Nextjs, Typescript, React-Redux, Tailwindcss,"
          about="E-commerce platform."
          site="https://qshopp.vercel.app/"
          frontendrepo="https://github.com/Makinde1034/Qshop"
        />
        <Project
          title="Glover-frontend task"
          tools="VueJs, VueX, scss, "
          about="Glover frontend engineer assessment"
          site="https://makinde-glover-task.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Glover-takehome-test"
        />
        <Project
          title="Pencil"
          tools="VueJs, VueX, scss, MogoDB, NodeJs "
          about="Knowledge sharing platform"
          site="https://pencill.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Pencil"
          backendrepo="https://github.com/Makinde1034/pencil-backend"
        />
        <Project
          title="Photohome"
          tools="VueJs, VueX, scss,"
          about="Web app that gets beautiful images from unsplash"
          site="https://photohome.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Photo-home"
        />
        <Project
          title="Vaultdefi"
          tools="ReactJs(Typscript), Apexchart, Redux css, Etherjs"
          about="Decentralised application that allows users to save different ethereum tokens and get a reward"
          site="https://vaultdefi.app/"
        />
        <Project
          title="Kpk-store"
          tools="VueJs"
          about="E-commerce website"
          site="https://kpk-store.netlify.app/"
        />
        <Project
          title="Form-plus task"
          tools="Reactjs(Typescript), scss, Redux"
          about="Formplus frontend assessment test."
          site="https://makinde-formplus-task.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Fromplus-task"
        />
        <Project
          title="Pacavel"
          tools="Reactjs, html,css,javascript"
          about="Software development agency website."
          site="https://pacavel.herokuapp.com/"
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
        <Project
          title="Pharmacy"
          tools="Nuxtjs"
          about="Drug prescription app."
          site="https://pharmacyapp-v2.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/phamarcyApp-v2"
        />
        <Project
          title="Sterling task"
          tools="Nextjs"
          about="Uncompleted project."
          site="https://sterlingtask.netlify.app/"
        />
        <Project
          title="Github-most-starred"
          tools="Vue3, composition API"
          about="A list of most starred gitub repositories with infinite scrolling."
          site="https://githhub-most-starred.netlify.app/"
          frontendrepo="https://github.com/Makinde1034/Vue-infinite-scroll-Composition-api"
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
