<template>
  <div id="not-found">
    <Inicio></Inicio>
    <div class="mt-5 text-center">
      <h4>Lo sentimos, la página que buscas no existe :(</h4>
    </div>
  </div>
</template>

<script>
import Inicio from '../components/Inicio.vue'

export default {
  name: 'NotFound',
  components: { Inicio }
}
</script>
<style></style>
