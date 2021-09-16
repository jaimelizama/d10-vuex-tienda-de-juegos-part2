<template>
  <div id="total" class="container">
    <Inicio></Inicio>
    <!-- Listado Total de Ventas -->
    <div class="mt-5 text-center">
      <h4>Listado Total de Ventas</h4>
      <Juegos :juegos="$store.state.ventas"></Juegos>
    </div>

    <!-- Monto Total de Ventas -->
    <div class="mt-5 text-center">
      <h4>Monto Total de Ventas</h4>
      <ul class="mt-3">
        <li>Monto Total: {{ $store.getters.montoTotalDeVentas }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
import Inicio from '../components/Inicio.vue'
import Juegos from '../components/Juegos.vue'
export default {
  components: { Inicio, Juegos },
  name: 'Total'
}
</script>

<style></style>
