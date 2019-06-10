<template>
  <v-app>
    <v-content>
      <router-view/>
      <navigation/>
    </v-content>
  </v-app>
</template>

<script>
import navigation from './components/navigation'
import Home from './views/Home'


export default {
  name: 'App',
  components: {
    navigation,
  },
  data () {
    return {
      //
    }
  }
}
</script>
