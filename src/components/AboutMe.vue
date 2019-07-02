<template>
  <section class="hide-overflow">
    <v-layout white>
      <v-flex xs12 md6 pa-5>
        <base-bubble-1 max-height=60 style="transform: translate(5%, -5%)" />
        <base-heading id="about" class="info--text">Nosotros</base-heading>

        <!-- <base-text class="mb-5">
          Lorem ipsum dolor sit amet, consectetur adipi
          <br />scin elit. Etiam vulputate augue vel felis gravida
          <br />porta. Lorem ipsum dolor sit amet.
        </base-text> -->

        <base-subheading class="info--text">Mision</base-subheading>
        <base-text class="mb-5">
          Somos un negocio innovador, que brinda servicios de catering. Ofreciendo una atención exclusiva, personalizada en estilo y diseño de acuerdo a tu necesidad, cuidando los más finos detalles, para que ese momento importante de tu vida se convierta en un día inolvidable.
        </base-text>

        <base-subheading class="info--text">Vision</base-subheading>
        <base-text class="mb-5">
          Ser reconocidos dentro la línea de CATERING más prestigiosas del mercado, basándonos en nuestros principios de “calidad de servicio rapidez e innovación”. Promoviendo trabajo y satisfacción las expectativas de nuestro cliente.
        </base-text>

        <base-subheading class="info--text">Valores</base-subheading>
        <v-alert >
          <v-layout v-for="(skill, i) in skills" :key="i" style="color: #69A1BB;" wrap>
            <v-flex xs12 text-uppercase v-text="skill" />
            <!-- <v-flex xs6 text-xs-right v-text="`${skill.value}%`" /> -->
            <!-- <v-progress-linear :value="skill.value" color="info" height="8" /> -->
          </v-layout>
        </v-alert>
      </v-flex>
      <v-flex hidden-sm-and-down md6>
        <v-img :src="require('@/assets/aboutme.png')" height="100%" />
      </v-flex>
    </v-layout>
  </section>
</template>

<script>
export default {
  data: () => ({
    skills: [
      "Honestidad",
      "Responsabilidad",
      "Dedicación",
      "Productividad",
      "Respeto",
      "Trabajo en equipo",
      "Alegría",
      "Optimismo",
    ]
  })
};
</script>
