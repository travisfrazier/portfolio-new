<template>
  <div class="layout">
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>


<style lang="scss">
 @font-face {
    font-family: 'Space Grotesk';
    src: url('../assets/fonts/SpaceGrotesk-VariableFont_wght.ttf');
    font-weight: normal;
}
html {
  overflow-x: hidden;
}

body {
  position: relative;
  font-family: 'Space Grotesk', sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
  background: $color-dark;
  color: $color-lightest;
  overflow-x: hidden;
}

.layout {
  max-width: 1110px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

button {
  font-size: 16px;
  background: none;
  border: none;
  border-bottom: 1px solid $color-bright;
  text-transform: uppercase;
  color: $color-lightest;
  font-weight: 700;
  letter-spacing: 2.29px;
  padding-bottom: 8px;
  padding: 0px 0px 8px 0px;
  cursor: pointer;
  &:hover {
    color: $color-bright;
  }
}
</style>
