<template>
  <div id="app">
      <table class="table table-dark text-center">
          <thead>
          <tr>
              <th>Nombre</th>
              <th>Apellido</th>
              <th>RUN</th>
              <th>Nacimiento</th>
              <th>Edad</th>
          </tr>
          </thead>
          <tbody>
          <tr v-for="(persona) of personas" :key="persona">
            <td>{{persona.nombre}}</td>
            <td>{{persona.apellido}}</td>
            <td>{{persona.run}}</td>
            <td>{{persona.fecha}}</td>
            <td>{{persona.edad}}</td>
          </tr>
          </tbody>
      </table>
  </div>
</template>

<script>
export default {
  name: "App",
  data: () => ({
    personas: [
      {
        nombre: "José",
        apellido: "Pérez",
        run: "10101010-1",
        fecha: "10-01-10",
        edad: "12"
      },
      {
        nombre: "María",
        apellido: "Rodríguez",
        run: "12345678-9",
        fecha: "30-11-90",
        edad: "32"
      },
      {
        nombre: "Manuel",
        apellido: "Patiño",
        run: "11223344-5",
        fecha: "02-12-59",
        edad: "63"
      }
    ]
  }) // cierre data
}; // cierre export default

</script>

<style></style>
