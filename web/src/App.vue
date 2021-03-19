<template>
  <v-app>
    <v-main>
      <Page/>
    </v-main>
  </v-app>
</template>

<script>
import Page from './components/Page'

export default {
  name: 'App',

  components: {
    Page
  },

  data: () => ({
    collapseOnScroll: true
  }),
};
</script>
