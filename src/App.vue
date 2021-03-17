<template>
  <svg-definitions></svg-definitions>
  <app-container></app-container>
</template>

<script>
import "./assets/fonts/fonts.css";
import SvgDefs from "./SvgDefs";
import AppContainer from "./components/AppContainer";

export default {
  name: "App",
  components: {
    "svg-definitions": SvgDefs,
    "app-container": AppContainer
  }
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

  @media only screen and (max-width: 1150px) {
    font-size: 50%;
  }
}

* {
  margin: 0;
  padding: 0;
}

/*
  Note:
    The following is a good strategy if you want to have everything set up to have a default
    box-sizing of border-box.
    You set box-sizing: border-box to the root html element and inherit to all the other elements,
    in this way every element gets border-box but it is still easy to change the box-sizing of
    elements and have the change propagate to their children.
*/
*,
*::before,
*::after {
  box-sizing: inherit;
}

body {
  background-image: linear-gradient(
    to right bottom,
    var(--color-primary-lighter),
    var(--color-primary-darker)
  );
}

#app {
  font-family: "OpenSans", sans-serif;
  font-weight: 400;
  line-height: 1.6;

  color: var(--color-gray-darker);

  min-height: 100vh;
  background-image: linear-gradient(
    to right bottom,
    var(--color-primary-lighter),
    var(--color-primary-darker)
  );
}
</style>
