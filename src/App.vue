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
  min-width: 1440px;
  height: 900px;
  /* overflow: hidden; */
  text-rendering: optimizeSpeed;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
}
</style>
