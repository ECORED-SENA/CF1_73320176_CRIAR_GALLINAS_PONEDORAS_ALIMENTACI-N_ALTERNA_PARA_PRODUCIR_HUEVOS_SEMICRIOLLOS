<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
import Actividad from 'ecored-pkg-fliz/plugin/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema:
        'Manejo integral operativo y sanitario en explotaciones avícolas de postura.',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> Evaluar la comprensión de los aprendices sobre los fundamentos biológicos, sanitarios y productivos en la crianza de gallinas ponedoras, mediante la resolución de preguntas de selección múltiple y verdadero o falso, que permitan identificar el nivel de conocimiento adquirido sobre anatomía aviar, bienestar animal, manejo sanitario, bioseguridad y sistemas de producción avícola.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO.',
      preguntas: [
        {
          id: 1,
          texto:
            '¿Cuál es el objetivo principal de la sanidad avícola en gallinas ponedoras?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aumentar el tamaño del huevo para mejorar su apariencia.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Prevenir, controlar y erradicar enfermedades en las aves.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto:
                'Reducir el consumo de alimento y así no padecer de sobrepeso.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Mejorar el color del plumaje para que tenga apariencia sana.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 2,
          texto:
            '¿Qué órgano del sistema digestivo aviar se encarga de triturar el alimento?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Molleja.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Esófago.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Buche.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Intestino grueso.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 3,
          texto: '¿Cuál es la función del ovario en la gallina ponedora?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Transportar el alimento.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Absorber nutrientes paulitamente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Producir los óvulos o yemas.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Triturar el alimento y procesarlo.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 4,
          texto:
            '¿Cuánto tiempo aproximadamente tarda la formación completa de un huevo en la gallina?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: '10–12 horas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: '15–18 horas.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: '24–26 horas.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: '30–36 horas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 5,
          texto:
            '¿Cuál de los siguientes comportamientos es natural en las gallinas y contribuye al bienestar animal?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Permanecer inmóviles todo el día.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Dormir en el suelo húmedo y tranquilamente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Escarbar el suelo en busca de alimento.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Evitar el contacto con otras aves y evitar riesgos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 6,
          texto:
            '¿Qué porcentaje aproximado de proteína se recomienda en la alimentación de gallinas ponedoras en sistemas semicriollos?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: '10–12 %.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: '16–18 %.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: '12–14 %.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: '22–24 %.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 7,
          texto:
            '¿Cuál es una conducta natural utilizada por las gallinas para controlar ectoparásitos?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Baños de alimento.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Baños de agua.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Baños de sombra.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Baños de polvo.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 8,
          texto:
            '¿Cómo se llama la estructura genética de la producción avícola que incluye abuelas, reproductoras y líneas comerciales?	Rta(s) correcta(s) (x)',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Cadena alimenticia.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Sistema sanitario.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Pirámide genética.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Programa de bioseguridad.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 9,
          texto:
            '¿Cuál es la función principal de las aves llamadas “reproductoras”?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Producir carne para consumo humano de la mejor calidad.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Producir huevos fértiles que originan pollitas comerciales.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto:
                'Producir alimento para otras aves para promover el desarrollo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Mejorar el plumaje de las aves.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 10,
          texto:
            '¿Qué sistema productivo permite mayor expresión de comportamientos naturales en las gallinas?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Jaula tecnificada y segura.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Sistema intensivo cerrado.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Sistema de traspatio o semicriollo.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Sistema industrial automatizado.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 11,
          texto:
            '¿Cuál de las siguientes enfermedades aviares es altamente contagiosa y causada por un virus?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Newcastle.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Salmonelosis.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Coccidiosis.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Colibacilosis',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 12,
          texto:
            '¿Qué institución en Colombia regula y supervisa la sanidad avícola?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Ministerio de Educación.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Policía Nacional.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'ICA (Instituto Colombiano Agropecuario).',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Ministerio de Transporte.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 13,
          texto:
            '¿Cuál es el objetivo principal de la bioseguridad en una granja avícola?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Aumentar el peso de las aves proporicionalmente hasta que logren su peso.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Reducir el consumo de alimento por salud y bienestar animal.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Prevenir la entrada y propagación de enfermedades.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Mejorar el color del huevo, tamaño y nutrientes en su producción.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 14,
          texto:
            '¿Cuál es la vía de administración más común para vacunas en aves recién nacidas contra Newcastle?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Intramuscular.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Ocular o spray.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Intravenosa.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Oral directa.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 15,
          texto:
            '¿Cuál es una característica de las gallinas criollas en comparación con las comerciales?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Mayor rusticidad y adaptación al ambiente.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Menor resistencia a enfermedades.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Mayor producción de huevos.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Menor capacidad de adaptación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 16,
          texto:
            '¿Por qué las gallinas ponedoras utilizan principalmente un solo ovario funcional?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Porque el otro ovario está dañado y no puede forzarlo ni afectarlo más.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Para reducir el peso corporal y facilitar el vuelo para realizar jerarquía.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Para optimizar la producción de huevos y eficiencia energética.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Porque nacen con un solo ovario y genéticamente no están aptas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 17,
          texto:
            '¿Cuál de las siguientes acciones contribuye al bienestar animal en aves?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                '¿Cuál de las siguientes acciones contribuye al bienestar animal en aves?',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Solo administrar medicamentos cuando enferman  o se requieran desparasitar.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Mantenerlas en espacios reducidos para controlarlas mejor.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Evitar el contacto con otras aves para que entre las de su misma raza se relacionen mejor.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 18,
          texto:
            '¿Cuál es un objetivo principal de la bioseguridad en granjas avícolas?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aumentar la velocidad de crecimiento de las aves.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reducir costos de alimentación.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Mejorar el color de los huevos.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Evitar la entrada y propagación de enfermedades.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 19,
          texto:
            '¿Qué característica distingue a las gallinas comerciales de las criollas?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Son más resistentes a todas las enfermedades.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Producen mayor cantidad de huevos al año.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'No requieren alimentación balanceada.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Viven menos tiempo, la mortalidad es alta.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 20,
          texto: '¿Cómo afecta el estrés a las gallinas ponedoras?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Mejora la calidad del huevo, mejora su tamaño y consistencia.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'No tiene ningún efecto, es indiferente y los factores externos no influyen.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Disminuye la producción y afecta la calidad del huevo.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Aumenta la producción de huevos de manera acelerada.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
