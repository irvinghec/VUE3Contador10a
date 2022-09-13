<script>
// export default {
//   data(){
//     return{
//       contador: 200,
//     };
//   },
// };
export default {
  data: () => ({
    contador: 500,
  }),
  methods: {
    saludar() {
      console.log("Hola 10A");
    },
    incrementar() {
      this.contador++;
    },
    decrementar() {
      this.contador--;
    },
    resetear() {
      this.contador = 0;
    },
  },
};
</script>
<template>
  <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125">
  <div class="container">
    <small>
      <h1>Hola desde VUE.js 3</h1>
    </small>
    <br />
    <h2>Contador {{ contador }}</h2>
    <br />
    <button @click="incrementar()">+1</button>
    <button @click="decrementar()">-1</button>
    <button @click="resetear()">Reset</button>
    <!-- Button trigger modal -->
    <button type="button" class="btn btn-primary" data-toggle="modal" data-target="#Modal">
      Barra emergente
    </button>
  </div>
<!-- Modal -->
<div class="modal fade" id="Modal" tabindex="-1" role="dialog" aria-labelledby="ModalLabel" aria-hidden="true">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="ModalLabel">Irving Henandez Carlos | DGS 10° "A"</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
        <div class="modal-body">
          <h6> VUE Deploy: Netlify, Vercel y GitHub</h6>
        </div>
    </div>
  </div>
</div>
</template>

<style scoped>
  .container {
    text-align: center;
  }
  small {
    color: #666;
  }
  h1 {
    font-weight: bolder;
  }
  h2 {
    font-size: 2.5rem;
  }
  button {
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 8px;
  }
  h5{
    color:midnightblue;
  }
  h6{
    color: gray;
  }
</style>