<template>
  <v-carousel
    cycle
    interval='3000'
    height="700"
    hide-delimiter-background
    show-arrows-on-hover
  >
    <v-carousel-item
      v-for="(obj, i) in slideObjs"
      :key="i"
      transition="fade-transition"
    >
      <v-sheet
        :color="obj.color"
        height="100%"
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
        <v-icon class='slideIcon
        mr-5
        text-h6
        text-sm-h4
        text-md-h3
        text-lg-h2'
        >
          {{ obj.icon }}
        </v-icon>
          <div class="
          text-h6
          text-sm-h4
          text-md-h3
          text-lg-h2"
          >
            {{ obj.text }}
          </div>

        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        slideObjs: [
          {
            color: 'indigo',
            text: ' Responsive website design',
            icon: 'mdi-web'
          },
          {
            color: 'deep-orange accent-3',
            text: ' Dynamic pages',
            icon: 'mdi-nodejs'
          },
          {
            color: 'green',
            text: ' Single page apps',
            icon: 'mdi-monitor-cellphone'
          },
          {
            color: 'deep-purple accent-4',
            text: ' Data visualizations',
            icon: 'mdi-language-python'
          },
          {
            color: 'blue darken-2',
            text: ' Social media integration',
            icon: 'mdi-account-search'
          },
        ],
      }
    },
  }
</script>

<style lang="css">
.slideIcon {
  font-size: 1.5em;
}
</style>
