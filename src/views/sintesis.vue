<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p.mb-5 El siguiente mapa conceptual integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo.

    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/template/sintesis/s-1.svg", alt="A continuación, se presenta la síntesis del componente formativo sobre Gestión Documental, que incluye los siguientes puntos: 1. Clasificación: esta es la primera fase, donde se prioriza la clasificación de documentos. Cada documento tiene su propia tipología y está compuesto por elementos. Esta fase se realiza siguiendo la normativa. 2. Validación Documental: en esta fase, se revisan documentos para su eliminación y migración. Ambos procesos requieren subprocesos, actas y herramientas ofimáticas. Posteriormente, se realiza un control y seguimiento. En este punto, los documentos pasan a ser retenidos durante tiempos específicos, que varían según si la documentación es física o digital. Esto se lleva a cabo mediante instrumentos como tablas de retención documental, asegurando procesos exitosos. La validación se realiza de acuerdo con la normativa. 3. Retención Documental: esta fase hace referencia al tiempo de conservación de los documentos.")
      .col-lg-3
        a.anexo.mb-4(:href="obtenerLink('/downloads/sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis 

</template>

<script>
export default {
  name: 'Sintesis',
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
