<template>
  <div id="ventas" class="container">
    <Inicio></Inicio>
    <!-- Cantidad de Juegos Disponibles -->
    <div class="mt-5 text-center">
      <h4>Cantidad de Juegos con Stock</h4>
      <ul class="mt-3">
        <li># Juegos: {{ $store.getters.juegosConStock }}</li>
      </ul>
    </div>
    <!-- Venta de Juegos -->
    <div class="mt-5 text-center">
      <h4>Venta de Juegos</h4>
      <Juegos
        :juegos="$store.state.juegos"
        modo="vender"
        @vender="$store.dispatch('venderJuego', $event)"
      ></Juegos>
    </div>
  </div>
</template>

<script>
import Inicio from '../components/Inicio.vue'
import Juegos from '../components/Juegos.vue'

export default {
  name: 'Ventas',
  components: { Inicio, Juegos }
}
</script>

<style></style>
