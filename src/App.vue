<template>
  <v-app>
    <!-- <v-app-bar app>
      <v-spacer></v-spacer> 
      <v-btn text to="/">Home</v-btn>
      <v-btn text to="/timetable">Time Table</v-btn>
      <v-btn text to="/contact">Contact Info</v-btn>
      <v-spacer></v-spacer>
    </v-app-bar> -->
    <v-main>
      <router-view/>
    </v-main>
    <v-footer class="footer-background">
    <v-row justify="center" class="footer-content">
      <v-btn icon href="https://www.tiktok.com/@coachmarvbjj" target="_blank" class="social-icon">
        <v-icon size="24">mdi-tiktok</v-icon>
      </v-btn>
      <v-btn icon href="https://www.instagram.com/coachmarvbjj/" target="_blank" class="social-icon">
        <v-icon size="24">mdi-instagram</v-icon>
      </v-btn>
      <v-btn icon href="https://www.facebook.com/martyn.oliver.75" target="_blank" class="social-icon">
        <v-icon size="24">mdi-facebook</v-icon>
      </v-btn>
    </v-row>
  </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    //
  }),
}
</script>
<style scoped>
.footer-background {
  padding: 20px 0;
  background-color: #15202b;
}

.footer-content {
  max-width: 500px;
  margin: auto;
}

.social-icon {
  margin: 0 10px;
}

</style>