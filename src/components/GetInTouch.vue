<template>
  <section id="get-in-touch" class="hide-overflow">
    <v-layout info white--text>
      <v-flex hidden-sm-and-down md6>
        <v-img :src="require('@/assets/contact.png')" height="100%" />
      </v-flex>
      <v-flex xs12 md6 pa-5>
        <base-bubble-1 max-height=100 />
        <base-heading class="mb-5">Contacto</base-heading>

        <v-sheet max-width="600" color="transparent">
          <v-text-field color="info" label="Nombres" solo flat />
          <v-text-field color="info" label="Email" solo flat />
          <v-text-field color="info" label="Asunto" solo flat />
          <v-textarea color="info" label="Mensaje" solo flat />
          <base-btn>Enviar</base-btn>
        </v-sheet>
      </v-flex>
    </v-layout>
  </section>
</template>
