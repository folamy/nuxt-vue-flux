<template>
  <section class="container">
    <div>
      <vue-flux
        :options="fluxOptions"
        :images="fluxImages"
        :transitions="fluxTransitions"
        ref="slider">
      </vue-flux>
    </div>
  </section>
</template>

<script>
import { VueFlux, Transitions } from 'vue-flux';

export default {
  components: {
      VueFlux
   },
 
   data: () => ({
      fluxOptions: {
         autoplay: true
      },
      fluxImages: [
         'images/material.jpg',
         'images/nigerian-schools-1024x483.jpg',
         'images/bck1.jpeg'
      ],
      fluxTransitions: {
         transitionBook: Transitions.transitionBook
      }
   })
}
</script>

<style>

</style>

