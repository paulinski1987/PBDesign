<template>
  <v-container class="about">

    <v-row>
      <v-col>
      <v-card
      color='blue darken-4'
      class='pa-8 bdr'
      outlined shaped>

        <v-container>
          <v-row>
            <v-col
              cols='12'
              md='6'
            >
            <v-img
              src='../assets/profilePic.png'
              class='profilePic'
              alt='picture of paul banks'
            ></v-img>
            <div class='text-title
              pt-5 ml-10
              black--text'
              style='margin-top: -5px; font-weight: bolder;'
            >
              Paul Banks
            </div>
            <div class='text-subtitle-2
              pa-0 ml-15
              light-green--text text--accent-3'
              style='margin-top: -5px; opacity: 0.5;'
            >
              Web developer
            </div>
            </v-col>

            <v-col
              cols='12'
              md='6'
            >
            <v-card-text class='txt white--text'>
              I was born in Calgary Albera as the oldest of 7 children. I grew up on a small hobby farm south of Calgary; it's a nice area with lots of wildlife despite its proximity to the city. We have sheep, chickens, bees and a large vegetable garden as well as a couple dogs and a cat.</v-card-text>
            <v-card-text class='txt white--text'>
              I enjoy a multitude of different music genres, almost anything except for country. My favorites genres are classical and metal. I love the outdoors and try to get out to the Rocky Mountains to hike and camp as often as I can. The view and proximity to the mountains is one of the best aspects to life in this area.</v-card-text>
            <v-card-text class='txt white--text'>
              I learned glazing in trade school, studied psychology in university and started coding a few years ago. </v-card-text>
          </v-col>
          </v-row>
        </v-container>

      </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  mounted() {
    document.title = "About";
  },
}
</script>

<style lang='css'>
  .profilePic {
    max-width: 250px;
    border: 2px solid #FFF;
    border-bottom-right-radius: 1em;
  }
.txt { line-height: 1.5em; letter-spacing: 0.2em; font-size: 1.2em;}
.about {
  max-width: 1200px;
  margin-top: 1em;
}
</style>
