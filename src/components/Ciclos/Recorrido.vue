<script>
export default {
  data() {
    return {
      //DATOS DE ALUMNO
      alumnos: [
        { nc: 21026, nombre: "Alvaro", Carrera: "ISC" },
        { nc: 21026, nombre: "Ariel", Carrera: "ISC" },
        { nc: 21026, nombre: "Maviel", Carrera: "ISC" },
        { nc: 21026, nombre: "Carmen", Carrera: "CIV" },
        { nc: 21026, nombre: "Coro", Carrera: "IND" },
        { nc: 21026, nombre: "Antonia", Carrera: "ISC" },
        { nc: 21026, nombre: "Tania", Carrera: "ADM" },
      ],
    };
  },
};
</script>
<template>
  <div class="container">
    <h3>Lista de Alumnos</h3>
    <ul>
      <li v-for="alumno in alumnos" :key="alumno.nc">
        <strong>{{ alumno.nombre }}</strong>
        <strong>{{ alumno.Carrera }}</strong>
      </li>
    </ul>
  </div>
</template>

<style>
h3 {
  color: black;
  background-color: aquamarine;
  border-radius: 15px;
  padding: 10px;
  align-items: center;
}
ul {
  list-style-type: none;
  padding: 0%;
}
li {
  color: red;
  background-color: blue;
  border-radius: 15px;
  padding: 10px;
  margin: 10px;
  text-align: center;
}
</style>
