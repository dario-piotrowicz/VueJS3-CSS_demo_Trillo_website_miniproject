<template>
  <h1>Trillo App</h1>
</template>

<script>
import "./assets/fonts/fonts.css";

export default {
  name: "App"
};
</script>

<style lang="scss">
@import "./variables.scss";

html {
  box-sizing: border-box;

  /*
    We set the font-size to 62.5%, so that we generally get 1rem === 10px
    which can help us reason around our measures

    We came up with 62.5% because, browsers by default have their font-size equal to 16px,
    and 10 is 62.5 percent of 16 ( 10/16 * 100 = 62.5 )
  */
  font-size: 62.5%;
}

* {
  margin: 0;
  padding: 0;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

#app {
  font-family: "OpenSans", sans-serif;
  font-weight: 400;
  line-height: 1.6;

  min-height: 100vh;
  background-image: linear-gradient(
    to right bottom,
    var(--color-primary-lighter),
    var(--color-primary-darker)
  );

  h1 {
    color: #fff;
  }
}
</style>
