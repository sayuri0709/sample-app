<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-side-icon @click="toggleSideMenu"></v-toolbar-side-icon>
      <v-toolbar-title class="headline text-uppercase">
        <span>マイアドレス帳</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
    </v-toolbar>
    <sideNav></sideNav>

    <v-content>
    </v-content>
  </v-app>
</template>

<script>
import { mapActions}  from 'vuex';
import sideNav from './components/sideNav';
export default {
  name: 'App',
  components: {
    sideNav
  },
  data () {
    return {
      //
    }
  },
  methods: {
    ...mapActions(['toggleSideMenu'])
  }
}
</script>