<template>
  <router-view />
</template>

<style>
/* Box sizing rules */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* Remove default margin */
body,
h1,
h2,
h3,
h4,
p,
ul,
li,
input,
button {
  margin: 0;
  padding: 0;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto,
    Helvetica Neue, Ubuntu, sans-serif;
  width: 100vw;
  height: 100vh;
  overflow-x: hidden;
  text-rendering: optimizeSpeed;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
}
</style>
