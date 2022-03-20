<template>
  <v-app>
    <v-card
    >
      <v-app-bar
        elevation="24"
        height='200px'
        dark
        prominent
        src='./assets/nasa2.png'
      >
        <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>

        <v-app-bar-title>Paul Banks
            <v-subheader class='subtitle-2 marginFix text--disabled'>Web Developer</v-subheader>
        </v-app-bar-title>


        <v-spacer></v-spacer>
        <v-btn
          icon
          href='https://github.com/paulinski1987'
          target='_blank'
          title='visit my github page'
        >
          <v-icon>mdi-github</v-icon>
        </v-btn>

        <v-btn
          icon
          href='https://discordapp.com/users/793235702564913224/'
          target='_blank'
          title='add me to discord'
        >
          <v-icon>mdi-discord</v-icon>
        </v-btn>

        <v-btn
          icon
          href='mailto:mathewp9876@gmail.com'
          target='_blank'
          title='shoot me an email'
        >
          <v-icon>mdi-at</v-icon>
        </v-btn>
      </v-app-bar>

      <v-navigation-drawer
        v-model="drawer"
        absolute
        temporary
        height="100vh"
        color='light-blue darken-4'
      >
      <v-list dense
              nav>
        <v-list-item v-for="item in links"
                     :key="item.title"
                     :to="item.to"
                     active-class="blue accent-3--text text--lighten-"
                     link>
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      </v-navigation-drawer>
    </v-card>

    <v-main>
      <router-view/>
    </v-main>
    <my-footer />
  </v-app>
</template>

<script>
import MyFooter from './components/MyFooter.vue';
export default {
  name: 'App',
  data: () => ({
    drawer: false,
     group: null,
     links: [
       { title: 'Home', icon: 'mdi-space-invaders', to: '/' },
       { title: 'Skills', icon: 'mdi-code-braces', to: '/skills' },
       { title: 'About', icon: 'mdi-robot', to: '/about' },
       { title: 'Contact', icon: 'mdi-chat', to: '/contact' }
     ],
  }),
  components: {
    MyFooter
  }
};
</script>

<style lang='css'>
/* bg is #121212 */
.marginFix {
  margin-top: 0;
  padding-top: 0;
  padding-left: 0;
  padding-bottom: 0.5em;
  height: 1.5em;
}
</style>
