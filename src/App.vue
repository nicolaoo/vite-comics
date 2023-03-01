<script>
import comicsHeader from './components/comics-header.vue';
import comicsMain from './components/comics-main.vue';
import comicsFooter from './components/comics-footer.vue';

export default {
  components: {
    comicsHeader,
    comicsMain,
    comicsFooter,

  }

}
</script>

<template>
  <body>
    <comicsHeader />
    <comicsMain />
    <comicsFooter />
  </body>
</template>

<style >
body {
  height: 100vh;
  width: 100vw;
}
</style>
