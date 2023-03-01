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
  <comicsHeader />
  <comicsMain />
  <comicsFooter />
</template>

<style >
body {
  height: 100vh;
  overflow-y: auto;
  overflow-x: hidden;
}

.container {
  margin: 0 auto;
  max-width: 900px;

}

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}


ul {
  list-style-type: none;
}

img {
  max-width: 100%;
}
</style>
