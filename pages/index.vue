<template>
  <transition name="home">
    <div class="home">
      <img src="../static/photo_2022-04-18_11-51-43.jpg" alt="" />
      <h3>Makinde Tolulope</h3>
      <p>
        Hi, I'm a software developer with experience building client facing
        software based on reusable patterns. I adhere to strict coding
        standards, conduct thorough testing, and implement best practices. I
        enjoy working with Typescript, Reactjs, Vuejs, React native and Golang.
        I also like exploring new programming languages and frameworks. I
        presently work at a fintech company that creates innovative solutions to
        transform the way people engage with finance.
      </p>
      <button @click="downloadMe">
        
          Download resume
        
      </button>
    </div>
  </transition>
</template>

<script>
export default {
  transition: 'home',
  data() {
    return {
      content: "Makinde Tolu's portfolio",
    }
  },
  head() {
    return {
      title: this.content,
      meta: [
        {
          hid: 'Makinde Tolulope',
          name: 'Makinde Tolulope ',
          content: this.content,
        },
      ],
    }
  },
  methods: {
    downloadMe() {
      const link = document.createElement('a')
      link.href = '/Makinde-tolulope-cv.pdf'
      link.download = 'Makinde-cv.pdf'
      link.target = '_blank'
      link.click()
    },
  },

}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Work+Sans&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  overflow-x: hidden;
}

body {
  background-repeat: no-repeat;
  background: linear-gradient(60deg, #000000f6, #000000ef),
    url(../static/image.jpg);
  background-size: cover;
}

.home {
  height: calc(100vh - 60px);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: white;
}

.home img {
  height: 200px;
  width: 200px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 30px;
}

.home h3 {
  font-size: 30px;
  margin-bottom: 10px;
  color: #f2de63;
  font-family: 'Work Sans', sans-serif;
}

.home p {
  font-family: 'Work Sans', sans-serif;
  text-align: center;
  width: 40%;
  line-height: 25px;
  font-size: 14px;
}

.home button {
  padding: 15px 15px;
  margin-top: 15px;
  border: 1px solid #f2de63;
  background: none;
  color: white;
  font-weight: bold;
  font-family: 'Work Sans', sans-serif;
  font-size: 12px;
  border-radius: 5px;
  cursor: pointer;
}

.home a {
  color: white;
  text-decoration: none;
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
  .home {
    padding: 0px 20px 0px 20px;
  }

  .home p {
    width: 100%;
    font-size: 12px;
  }
}

@media screen and (min-width: 480px) and (max-width: 768px) {
  .home {
    padding: 0px 20px 0px 20px;
  }

  .home p {
    width: 70%;
  }
}
</style>
