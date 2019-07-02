<template>
  <section id="welcome" class="hide-overflow">
    <v-layout>
      <v-flex hidden-sm-and-down md6>
        <v-img src="catering-eventos-barzola.jpg" height="100vh" />
      </v-flex>

      <v-flex
        xs12
        md6
        align-content-space-between
        layout
        :pa-5="$vuetify.breakpoint.smAndDown"
        wrap
      >
        <base-bubble-1 style="transform: rotate(180deg) translateY(25%)" />

        <v-layout align-content-start justify-center>
          <v-flex xs10 md6>
            <base-heading class="mt-0">Eventos Barzola!</base-heading>
            <base-text>Cumplimos todos tu sueños.</base-text>
            <base-btn class="mt-4">Leer mas!</base-btn>
          </v-flex>
        </v-layout>

        <base-bubble-2 style="transform: rotate(180deg) translate(-200px, -15%)" />
      </v-flex>
    </v-layout>
  </section>
</template>
