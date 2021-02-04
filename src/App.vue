<template>
  <h1>Trillo App</h1>
</template>

<script>
export default {
  name: "App"
};
</script>

<style lang="scss">
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
  h1 {
    color: green;
  }
}
</style>
