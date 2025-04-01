<script>
export default {
  data() {
    return {
      display: '',
      currentValue: 0,
    };
  },
  methods: {
    agregarNumero(numero) {
      this.display += numero;
    },

    calculo() {
      try {
        this.currentValue = new Function(`return ${this.display}`)();
        this.display = this.currentValue.toString();
      } catch (error) {
        this.display = "Error";
      }
    },

    Limpiardisplay() {
      this.display = '';
    },

    EliminarNumero() {
      this.display = this.display.slice(0, -1);
    },

    calcularPorcentaje() {
      if (this.display !== '' && !isNaN(parseFloat(this.display))) {
        this.display = (parseFloat(this.display) / 100).toString();
      }
    }
  }
};
</script>

<template>
  <div class="container d-flex justify-content-center mt-4" style="height: 350px;">
    <div class="card p-3" style="width: 300px; background-color: red;">
      <div class="card-body">
        <h6 class="text-center">Calculadora V2</h6>

        <!-- Display de la calculadora -->
        <div class="mb-3">
          <input type="text" class="form-control" v-model="display" disabled>
        </div>

        <!-- Botones de la calculadora -->
        <div class="d-flex justify-content-between gap-3 mt-2">
          <button class="btn btn-warning flex-fill px-2" @click="calcularPorcentaje()">%</button>
          <button class="btn btn-danger flex-fill px-1" @click="Limpiardisplay()">CE</button>
          <button class="btn btn-danger flex-fill px-2" @click="Limpiardisplay()">C</button>
          <button class="btn btn-danger flex-fill px-2" @click="EliminarNumero()">B</button>
        </div>

        <div class="d-flex justify-content-between gap-3 mt-2">
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(7)">7</button>
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(8)">8</button>
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(9)">9</button>
          <button class="btn" style="background-color: orange; color: white;" @click="agregarNumero('/')">/</button>
        </div>

        <div class="d-flex justify-content-between gap-3 mt-2">
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(4)">4</button>
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(5)">5</button>
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(6)">6</button>
          <button class="btn" style="background-color: orange; color: white;" @click="agregarNumero('*')">*</button>
        </div>

        <div class="d-flex justify-content-between gap-3 mt-2">
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(1)">1</button>
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(2)">2</button>
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(3)">3</button>
          <button class="btn" style="background-color: orange; color: white;" @click="agregarNumero('-')">-</button>
        </div>

        <div class="d-flex justify-content-between gap-3 mt-2">
          <button class="btn btn-primary flex-fill px-2" @click="calculo()">=</button>
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero(0)">0</button>
          <button class="btn" style="background-color: gold; color: black;" @click="agregarNumero('.')">.</button>
          <button class="btn" style="background-color: orange; color: white;" @click="agregarNumero('+')">+</button>
        </div>
      </div>
    </div>
  </div>
</template>