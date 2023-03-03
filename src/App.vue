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

<style lang="scss">
@use './style/general.scss'
</style>
