<template>
  <div class="container my-4">
    <!-- Inyectando variables en el DOM -->
    <h1 class="text-primary">Bienvenidos a {{ titulo }}</h1>
    <h3 class="text-secondary">Subtitulo 1</h3>

    <!-- Usando v-bind -->
    <h3 v-bind:class="textWarning">Subtitulo 2 con v-bind</h3>
    <h3 :class="textInfo">Subtitulo 2 con v-bind simplificado</h3>

    <!-- Uso del operador ternario -->
    <h3>
      {{ (estado) ? 'El estado es verdadero (operador ternario)' : 'El estado es falso (operador ternario)'}}
    </h3>

    <!-- v-if v-else-if v-else -->
    <h3 v-if="estadoVif">El estado es verdadero (usando v-if)</h3>
    <h3 v-else>El estado es falso (usando v-if)</h3> <!-- Ambas comprobaciones v-else y v-else-if deben estar adyacentes -->

    <h3 class="text-danger" v-if="estadoVifElseif === true">El estado es verdadero (usando v-if y v-else-if)</h3>
    <h3 class="text-danger" v-else-if="estadoVifElseif === false">El estado es falso (usando v-if y v-else-if)</h3>
    <h3 class="text-danger" v-else>El estado es otro (usando v-if y v-else-if)</h3>


    <!-- v-for -->
    <h3 class="text-primary">{{ paises }}</h3>

  </div>
</template>

<script setup>
  // Variable a inyectar en el DOM
  const titulo = 'Vue JS 3.0';

  // Uso de v-bind
  const textWarning = 'text-warning';
  const textInfo = 'text-info';

  // Uso del operador ternario
  const estado = true;

  // Uso de v-if
  const estadoVif = false;
  const estadoVifElseif = null;

  // Uso del v-for
  const paises = ['Argentina', 'Brasil', 'Venezuela'];

</script>

<style>

</style>