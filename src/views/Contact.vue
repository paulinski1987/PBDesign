<template lang="html">
  <v-container>
    <v-row class='mt-10'>
      <v-col
        cols='12'
        lg='6'
      >
        <v-card
          elevation='10'
          shaped
          outlined
          class='fill-height'
        >
          <v-card-title>
            <v-avatar size='60'>
              <v-img
                src='../assets/profilePic.png'
                class='profilePic mr-5'
                alt='picture of paul banks'
              ></v-img>
            </v-avatar>
            Contact Information
          </v-card-title>

          <v-divider></v-divider>
          <v-card-text>
            <a
            href='https://github.com/paulinski1987'
            target='_blank'
            title='visit my github page'
            ><v-icon class='mr-4'>mdi-github</v-icon> Github Profile</a>
          </v-card-text>

          <v-divider></v-divider>
          <v-card-text>
            <a
            href='https://discordapp.com/users/793235702564913224/'
            target='_blank'
            title='add me to discord'
            ><v-icon class='mr-4'>mdi-discord</v-icon> Discord Profile</a>
          </v-card-text>

          <v-divider></v-divider>
          <v-card-text>
            <a
            href='mailto:mathewp9876@gmail.com'
            target='_blank'
            title='shoot me an email'
            ><v-icon class='mr-4'>mdi-at</v-icon> mathewp9876@gmail.com</a>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col
        cols='12'
        lg='6'
      >
        <v-card
          elevation='10'
          outlined
        >
        <v-card-title>My personal thanks to:</v-card-title>
        <v-simple-table>
          <template v-slot:default>
            <thead>
              <tr>
                <th class="text-left">
                  Who
                </th>
                <th class="text-left">
                  What
                </th>
                <th class="text-left">
                  Where
                </th>
              </tr>
            </thead>
            <tbody>
              <tr
              >
                <td>NASA</td>
                <td>Navbar image</td>
                <td><a href='https://www.nasa.gov/' target='_blank'>NASA Official Website</a></td>
              </tr>

              <tr
              >
                <td>Vue</td>
                <td>Application framework</td>
                <td><a href='https://vuejs.org/' target='_blank'>Vue - The progressive Javascript Framework</a></td>
              </tr>

              <tr
              >
                <td>Vuetify</td>
                <td>Styling components</td>
                <td><a href='https://vuetifyjs.com/' target='_blank'>Vuetify - Material Design Framework</a></td>
              </tr>

              <tr
              >
                <td>Free Code Camp</td>
                <td>Educational Material</td>
                <td><a href='https://www.freecodecamp.org/' target='_blank'>Learn To Code For Free</a></td>
              </tr>

              <tr
              >
                <td>Udemy</td>
                <td>Educational Material</td>
                <td><a href='https://www.udemy.com' target='_blank'>Udemy - Best-Selling Online Courses</a></td>
              </tr>
            </tbody>
          </template>
        </v-simple-table>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    mounted() {
      document.title = "Contact";
    },
  }
</script>

<style lang="css">
a {
  text-decoration: none;
  color: blue;
}

</style>
