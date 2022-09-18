<script>
  export default {
    data: () => ({
      contador: 500, 
    }),
    methods: {
      incrementar() {
        this.contador++;

      }, 
      disminuir() {
        this.contador--;
      },
      resetear() {
        this.contador=500;
      },
    },
  };
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="Vue.js">
    <small><h1> .... </h1></small>
    <hr />

    <h2>Contador {{contador}} </h2>

    <button @click="incrementar()"> +1</button>
    <button @click="disminuir()">-1</button>
    <button @click="resetear()">resetear</button>

      <!-- Button trigger modal -->
    <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
      Jessica M
    </button>

    <!-- Modal -->
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title" id="exampleModalLabel">Jessica M</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body">
            Desarrollo de Software 4toB
          </div>
          <div class="modal-footer">
            <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>