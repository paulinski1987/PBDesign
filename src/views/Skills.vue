<template lang="html">
  <div class="component-wrapper">
    <slides class='mt-5 mb-5'/>
  </div>
</template>

<script>
  import Slides from '../components/Slides.vue';
  export default {
    components: {
      Slides
    },
    mounted() {
      document.title = "Skills";
    },
  }
</script>

<style lang="css">
</style>
