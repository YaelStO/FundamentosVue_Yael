<template>
  <div class="container">
    <h3>Horario de Clases de Yael</h3>
    <table class="table">
      <thead>
        <tr>
          <th scope="col">Hora</th>
          <th scope="col">Lunes</th>
          <th scope="col">Martes</th>
          <th scope="col">Miercoles</th>
          <th scope="col">Jueves</th>
          <th scope="col">Viernes</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(row, index) in horario" :key="index">
            <td>{{ row.hora }}</td>
            <td>{{ row.lunes }}</td>
            <td>{{ row.martes }}</td>
            <td>{{ row.miercoles }}</td>
            <td>{{ row.jueves }}</td>
            <td>{{ row.viernes }}</td>

        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
import {ref} from 'vue';

const horario=ref ([
    {hora:'7:00 - 9:00', lunes:'Simulacion', martes:'IA', miercoles: 'Libre', jueves:'Simulacion', viernes:'Club'},
    {hora:'11:00-01:00', lunes:'Libre', martes:'Libre', miercoles: 'Libre', jueves:'IA', viernes:'Simulacion'},
    {hora:'1:00 - 3:00', lunes:' Ing. Sofware ', martes:'Libre', miercoles: ' Programacion WEB ', jueves:' Adm. de Base de Datos ', viernes:' Ing. Sofware'},
    {hora:'3:00 - 5:00', lunes:' Programacion WEB ', martes:'Libre', miercoles: ' Ing. Sofware ', jueves:'Libre', viernes:' Programacion WEB/Adm. de Base de Datos'},
    {hora:'5:00 - 7:00', lunes:' Adm. de Base de Datos ', martes:' Lenguajes de Interfaz ', miercoles: 'Libre', jueves:' Lenguajes de Interfaz ', viernes:'Libre'}
])

</script>