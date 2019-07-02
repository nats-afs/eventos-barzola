<template>
  <section class="hide-overflow">
    <v-layout>
      <v-flex xs12 md6 primary text-xs-center pa-5 white--text>
        <base-bubble-1 max-height="100" style="transform: rotate(180deg) translateX(25%)" />
        <base-heading id="recent-projects">Galeria</base-heading>

        <base-text class="mb-5">Gracias por la confianza a todos nuestros clientes.</base-text>

        <v-card color="secondary">
          <v-container grid-list-md pa-2>
            <v-layout wrap>
              <v-flex v-for="project in projects" :key="project" xs12 md6>
                <a href="#">
                  <v-img :src="`${project}.jpg`" max-height="300" />
                </a>
              </v-flex>
            </v-layout>
          </v-container>
        </v-card>
      </v-flex>
      <v-flex hidden-sm-and-down md6>
        <v-img :src="require('@/assets/recentprojects.png')" height="100%" />
      </v-flex>
    </v-layout>
  </section>
</template>

<script>
export default {
  data: () => ({
    projects: [
      "img0",
      "img1",
      "img2",
      "img3",
      "img4",
      // 'img5',
      "img6"
      // 'img7',
    ]
  })
};
</script>
