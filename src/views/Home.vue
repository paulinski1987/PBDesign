<template>
<div class='homeContainer ma-12'>
  <div class='gridAreaC'>
    <h1 class=' text-center green--text text--accent-4 text-h2'>
       Welcome!</h1>
           <p class='light-blue--text text--lighten-2'>
             Welcome to <strong class='purple--text'>Paul Banks designs</strong>, glad to have you here! Let me give you the 10&cent; tour. On the <span class='purple--text'>homepage</span> you will find news and announcements.
              The <span class='purple--text'>About</span> page has a short bio about me.
              The <span class='purple--text'>Skills</span> section has a slideshow summary of some of the dev stuff I have to offer. Last but not least is the <span class='purple--text'>Contact</span> page where you can ... you guessed it ... find out how to get ahold of me.
           </p>
           <p class='light-blue--text text--lighten-2'>
             On the top right and bottom center are links to my github page, email and Discord profile should you want to add me.
           </p>
           <p class='light-blue--text text--lighten-2'>
             Thanks and enjoy! - Paul Banks 2022
           </p>
  </div>
  <div class='gridAreaI'>
    <v-img src='../assets/browserClean.svg' />
  </div>

</div>
</template>

<script>
// // @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  mounted() {
    document.title = "Home";
  },
};
</script>
<style>
p { line-height: 1.5em; letter-spacing: 0.2em; font-size: 1.2em;}
h1 { letter-spacing: 0.25em; }
.homeContainer {
  display: grid;
  grid: "C I" 100%
        / 2fr 1fr;
  margin: auto 120px;
}
.gridAreaC {
  grid-area: 'C';
  text-align: center;
  margin: auto;
}
.gridAreaI {
  grid-area: 'I';
  max-width: 600px;
}

@media only screen and (max-width: 900px){
  .homeContainer {
    grid: "C"
          "I";
      margin: auto 40px;
  }
}
</style>
