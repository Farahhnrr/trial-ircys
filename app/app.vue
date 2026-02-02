<template>
  <NuxtPage />
</template>

<script setup>
</script>

<style>
@font-face {
  font-family: "Erode";
  src: url("/font/erode/Erode-Regular.otf") format("opentype");
  font-weight: 400;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "Erode";
  src: url("/font/erode/Erode-Medium.otf") format("opentype");
  font-weight: 500;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "Erode";
  src: url("/font/erode/Erode-Semibold.otf") format("opentype");
  font-weight: 600;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "Erode";
  src: url("/font/erode/Erode-Bold.otf") format("opentype");
  font-weight: 700;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "Inter";
  src: url("/font/inter/Inter-VariableFont_opsz,wght.ttf") format("truetype");
  font-weight: 100 900;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "Inter";
  src: url("/font/inter/Inter-Italic-VariableFont_opsz,wght.ttf") format("truetype");
  font-weight: 100 900;
  font-style: italic;
  font-display: swap;
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

body {
  margin: 0;
  background: #f3f2ed;
  color: #3a342c;
  font-family: "Inter", "Segoe UI", sans-serif;
}
</style>
