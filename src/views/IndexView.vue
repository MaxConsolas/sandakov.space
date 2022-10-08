<template>
  <div class="main">
    <h1>Hello <span class="emoji-hand">👋</span></h1>
    <p style="font-weight: 500; font-size: 2.2em">My name is Maxim Sandakov</p>
    <p>
      I am <span v-text="yearsOld"></span> years old.
      I have been doing programming for about <span v-text="yearsXp"></span> years, trying out different technologies.
      I have been engaged in industrial development for <span v-text="yearsWork"></span> years, in particular in PHP/JS.
    </p>
    <p>
      I have experience in SPA development, creating API's, create an MVC applications and deploy a server.
      In addition, I worked closely with Vue and Laravel frameworks.
    </p>
    <p>
      Outside of programming I enjoy video games and do <a href="https://500px.com/p/sandakov2016?view=photos"
        style="color: rgb(0, 37, 85);">photography</a>
    </p>
  </div>
</template>

<script>
export default {
  data() {
    return {
    }
  },
  computed: {
    yearsOld() {
      return new Date(new Date() - new Date(1998, 7, 4)).getUTCFullYear() - 1970;
    },
    yearsXp() {
      return new Date(new Date() - new Date(2016, 8, 1)).getUTCFullYear() - 1970;
    },
    yearsWork() {
      return new Date(new Date() - new Date(2018, 8, 1)).getUTCFullYear() - 1970;
    },
  },
}
</script>

<style>
.main {
  font-family: 'Rubik', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue',
    sans-serif;
  font-size: calc(10px + 0.33vw);
  -webkit-font-smoothing: antialiased;
  padding: 5vh 10vw;
  color: #121314;
}

h1 {
  font-size: 4.5em;
  font-weight: 500;
  margin-bottom: 0;
}

p {
  font-size: 1.6em;
  font-weight: 300;
  line-height: 1.4;
  max-width: 28em;
}

a {
  text-decoration: none;
  color: #121314;
  position: relative;
}

.emoji-hand {
  transition: all 0.5 ease-in-out;
  transform-origin: bottom right;
  display: inline-block;
}

.emoji-hand:hover {
  animation-duration: 1s;
  animation-name: hand-greeting;
}

@keyframes hand-greeting {
  from {
    transform: rotate(0deg);
  }

  33% {
    transform: rotate(-15deg);
  }

  66% {
    transform: rotate(15deg);
  }

  to {
    transform: rotate(0deg);
  }
}
</style>