<template>
  <v-footer dark padless>
    <v-card flat tile
            class="light-blue darken-4 white--text text-center fullWidth">
      <v-card-text class='pa-0 ma-0'>
        <span>{{ new Date().getFullYear() }} — <strong>Paul Banks Web Designs</strong></span>
        <v-btn v-for="icon in icons"
               :key="icon.ic"
               :href='icon.href'
               target='_blank'
               class="mx-4 white--text"
               icon>
          <v-icon size="24px">
            {{ icon.ic }}
          </v-icon>
        </v-btn>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        { ic: 'mdi-github', href: 'https://github.com/paulinski1987' },
        { ic: 'mdi-discord', href: 'https://discordapp.com/users/793235702564913224/' },
        { ic: 'mdi-at', href: 'mailto:mathewp9876@gmail.com' }
      ]
    })
  }
</script>

<style lang="css">
  .fullWidth {
    width: 100vw;
  }
</style>
