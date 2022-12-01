<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="Logo Vue.js" width="125" height="125">
    <small>
      <h1>Hola Mundo Desde Vue.js 3</h1>
    </small>
    <hr />

    <h2>Contador: {{ contador }}</h2>
    <button @click="aumentar()">+1</button>
    <button @click="disminuir()">-1</button>
    <button @click="reset()">Reset</button>
  </div>
  
</template>

<style scoped>
  .container{
    text-align: center;
  }
  h1{
    font-weight: bolder;
  }

  small{
    color: #666;
  }

  h2{
    font-size: 2.5rem;
  }

  button{
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0 6px;
  }
</style>

<script>
export default {
  data: () => ({
    contador: 10,
  }),
  methods: {
    aumentar(){
      this.contador++;
    },
    disminuir(){
      this.contador--;
    },
    reset(){
      this.contador = 10;
    }
  }
}
</script>
