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
      Outside of programming I enjoy video games and investment</a>
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
/* cyrillic-ext */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 300;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nMrXyi0A.woff2) format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
/* cyrillic */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 300;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nFrXyi0A.woff2) format('woff2');
  unicode-range: U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
/* hebrew */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 300;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nDrXyi0A.woff2) format('woff2');
  unicode-range: U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
/* latin-ext */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 300;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nPrXyi0A.woff2) format('woff2');
  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
/* latin */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 300;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nBrXw.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
/* cyrillic-ext */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 500;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nMrXyi0A.woff2) format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
/* cyrillic */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 500;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nFrXyi0A.woff2) format('woff2');
  unicode-range: U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
/* hebrew */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 500;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nDrXyi0A.woff2) format('woff2');
  unicode-range: U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
/* latin-ext */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 500;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nPrXyi0A.woff2) format('woff2');
  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
/* latin */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 500;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nBrXw.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
/* cyrillic-ext */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 700;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nMrXyi0A.woff2) format('woff2');
  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
}
/* cyrillic */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 700;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nFrXyi0A.woff2) format('woff2');
  unicode-range: U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}
/* hebrew */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 700;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nDrXyi0A.woff2) format('woff2');
  unicode-range: U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
}
/* latin-ext */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 700;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nPrXyi0A.woff2) format('woff2');
  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
/* latin */
@font-face {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 700;
  src: url(https://fonts.gstatic.com/s/rubik/v19/iJWKBXyIfDnIV7nBrXw.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}


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
