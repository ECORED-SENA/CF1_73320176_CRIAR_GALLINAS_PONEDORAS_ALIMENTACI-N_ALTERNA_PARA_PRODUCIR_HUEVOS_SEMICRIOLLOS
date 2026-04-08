<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción
    .row.justify-content-center.align-items-stretch.mb-5
      .col-lg-5.bg-color-5.p-4.p-md-5.d-flex.align-items-center.rounded-4(data-aos="fade-right")
        p.mb-0 La producción de huevo en avicultura requiere conocimientos técnicos, sanitarios y zootécnicos que garanticen el bienestar de las aves, la eficiencia productiva y el cumplimiento de normas de bioseguridad. Para ello, es necesario aplicar prácticas adecuadas de manejo, alimentación, vacunación y control sanitario.
      .col-lg-3.px-0(data-aos="zoom-in")
        figure.mb-0.h-100
          img.w-100.h-100(src='@/assets/curso/intro/img1.png' style="object-fit: cover; display:block;")
      .col-lg-4.ps-4.pe-4.pt-4.pt-md-5.pb-0.d-flex.flex-column.justify-content-end(data-aos="fade-left")
        .content-wrap
          img.mb-4(src="@/assets/curso/fondos/icono.svg", alt="Icono" style="width:70px").d-none.d-xl-block         
          p.mb-0 Además, el seguimiento del peso corporal, la viabilidad del lote y el uso responsable de medicamentos permiten prevenir enfermedades y mejorar la productividad, contribuyendo a sistemas de producción avícola sostenibles y a la obtención de huevos de calidad. 
</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
