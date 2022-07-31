<template>
  <div class="container">
    <div v-if="step1">
      <h1 class="title">Bienvenid@ a CAHIER 😃!</h1>
      <h3 class="subtitle">Antes de comenzar, queremos saber de vos!</h3>
      <form>
        <label class="label"> ¿Cuál es tu nombre? 🤔 </label>
        <input v-model="userName" class="input" type="text" placeholder="Nombre">
      </form>
      <button style="margin-top: 50px; width: 150px;" class="btn-carrito" v-on:click="continuar()"> Continuar >> <i class="fa-solid fa-angle-right"></i></button>
    </div>
    <div v-if="step2">

    </div>
  </div>
</template>

<script>
import Swal from 'sweetalert2'
import store from '../store/index'

let step1 = true
let step2 = false


export default {
  name: 'HomeView',
  components: {
  
  },
  data (){
    return {
      store: store.state,
      step1,
      step2,
      userName: '',
    }
  },
  methods: {
    continuar () {
      if (this.userName != ''){
        this.step1 = false
        let user = JSON.stringify(this.userName)
        localStorage.setItem("user", user)
        this.step2 = true
        console.log(localStorage.getItem("user"))
      } else {
        Swal.fire('Ups! Completa tu nombre para continuar')
      }
      
    }
  }
}
</script>

<style>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 500px;
  padding: 10px;
  background-image: url('https://img.freepik.com/free-vector/hand-painted-watercolor-floral-background_79603-1868.jpg?w=2000');
  background-size: cover;
}
.title {
  margin-bottom: 20px;
  color: #854e0f;
}
.subtitle {
  margin-bottom: 50px;
  color: #854e0f;
}
.label {
  font-weight: 700;
  margin-right: 20px;
}
.btn-carrito:disabled {
  background-color: grey ;
}
</style>