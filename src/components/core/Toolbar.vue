<template>
  <v-toolbar v-scroll="onScroll" :color="isTransparent ? 'transparent' : '#F5F5F5'" app flat>
    <v-toolbar-side-icon></v-toolbar-side-icon>
    <v-toolbar-title>Eventos Barzola</v-toolbar-title>
    <v-spacer />
    <v-toolbar-items class="hidden-sm-and-down">
      <v-btn flat @click="$vuetify.goTo('#welcome', options)">Inicio</v-btn>
      <v-btn flat @click="$vuetify.goTo('#about', options)">Nosotros</v-btn>
      <v-btn flat @click="$vuetify.goTo('#services', options)">Servicios</v-btn>
      <v-btn flat @click="$vuetify.goTo('#recent-projects', options)">Galeria</v-btn>
      <v-btn flat @click="$vuetify.goTo('#get-in-touch', options)">Contacto</v-btn>
    </v-toolbar-items>
    <SocialMedia class="hidden-sm-and-down"/>
  </v-toolbar>
</template>

<script>
export default {
  components: {
    SocialMedia: () => import("@/components/SocialMedia")
  },

  data: () => ({
    isTransparent: true,
    options: {
      duration: 600,
      offset: 0,
      easing: 'easeInOutQuart'
    }
  }),

  methods: {
    onScroll() {
      this.isTransparent = window.pageYOffset < 200;
    }
  }
};
</script>
