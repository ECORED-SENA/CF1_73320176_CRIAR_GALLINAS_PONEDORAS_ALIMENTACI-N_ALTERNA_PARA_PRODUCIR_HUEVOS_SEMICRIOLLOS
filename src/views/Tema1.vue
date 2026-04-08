<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 1
      h1 Fundamentos biológicos y productivos
    .row.justify-content-center.align-items-stretch.mb-3.g-0.bg-color-6
      .col-lg-5.d-flex
        figure.mb-0.w-100
          img.h-100.w-100(src='@/assets/curso/tema1/img1.png', style="object-fit: cover;")
      .col-lg-7.bg-color-purple-light.d-flex.align-items-center.p-4.p-lg-5
        p.mb-0 En este apartado se presentan los fundamentos biológicos y productivos de las gallinas ponedoras, abordando temas como la anatomía aviar, la etología y el bienestar animal, los modelos de bienestar en avicultura, las etapas de desarrollo, las razas y líneas de ponedoras, y los criterios para la selección de gallinas criollas. 
    Separador
    //- Inicio Tema1.1
    .row.mt-5
        #t_1_1.titulo-segundo.color-acento-contenido(data-aos="fade-right")
          h2 1.1 Anatomía aviar básica externa e interna
    p(data-aos="fade-left") La anatomía de las aves ponedoras está adaptada a la producción de huevos y a una digestión eficiente; comprenderla permite un manejo sanitario y zootécnico adecuado.
    //- Título con imagen
    .bg-full-width.mt-5
      .px-4.px-md-5.pb-md-3
      .titulo-con-imagen.mb-5(data-aos="fade-right")
        .titulo-con-imagen__fondo
          img.titulo-con-imagen__imagen(src="@/assets/curso/fondos/imagen-titulos.svg")
          h3.titulo-con-imagen__texto Anatomía externa del ave
    //- Título con imagen
    p(data-aos="fade-left") La anatomía externa de la gallina ponedora permite identificar estructuras visibles clave para evaluar su estado sanitario, bienestar y desempeño productivo en sistemas avícolas. Las partes principales son:
    //- Pestanas horizontales
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
        TabsC.color-acento-contenido.mt-1
          .py-3.py-md-4(titulo="Cabeza")
            .row
              .col-md-6
                figure
                  img(src='@/assets/curso/tema1/pestana01_1.png')
              .col-md-6.mb-4.mb-md-0
                h4 Cabeza
                p Pico, cresta, barbillas, ojos, orificios nasales.
          .py-3.py-md-4(titulo="Cuello")
            .row
              .col-md-6.mb-4.mb-md-0
                figure
                  img(src='@/assets/curso/tema1/pestana01_2.png')
              .col-md-6
                h4 Cuello
                p Estructura flexible que conecta cabeza y tronco del ave.
          .py-3.py-md-4(titulo="Tronco")
            .row
              .col-md-6.mb-4.mb-md-0
                figure
                  img(src='@/assets/curso/tema1/pestana01_3.png')
              .col-md-6
                h4 Tronco
                p Parte central del cuerpo donde se ubican órganos vitales.
          .py-3.py-md-4(titulo="Alas")
            .row
              .col-md-6.mb-4.mb-md-0
                figure
                  img(src='@/assets/curso/tema1/pestana01_4.png')
              .col-md-6
                h4 Alas
                p Extremidades que permiten equilibrio, desplazamiento y regulación térmica.
          .py-3.py-md-4(titulo="Patas")
            .row
              .col-md-6.mb-4.mb-md-0
                figure
                  img(src='@/assets/curso/tema1/pestana01_5.png')
              .col-md-6
                h4 Patas
                p Extremidades que permiten sostén, locomoción y escarbar alimento.
          .py-3.py-md-4(titulo="Cloaca")
            .row
              .col-md-6.mb-4.mb-md-0
                figure
                  img(src='@/assets/curso/tema1/pestana01_6.png')
              .col-md-6
                h4 Cloaca
                p Abertura común para excreción y reproducción en aves.
    //- Cierres Pestanas horizontales
    p(data-aos="fade-left") La importancia productiva de las estructuras externas radica en su capacidad para reflejar el estado sanitario, nutricional y funcional de las gallinas ponedoras en producción, tales como:



    //- Fin Tema1.1

 
</template>

<script>
export default {
  name: 'Tema1',
  data: () => ({
    mostrarIndicadorTarjetaAudio: true,
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
