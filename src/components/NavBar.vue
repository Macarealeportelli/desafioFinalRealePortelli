<template>
  <div class="container-gral shadow-sm p-3 mb-5 bg-body rounded">
    <a style="margin-left: 20px" class="navbar-brand" href="#">
      <img src="/docs/5.2/assets/brand/bootstrap-logo.svg" alt="" width="30" height="24">
    </a>
    <form class="d-flex" role="search">
      <input class="input" type="search" placeholder="Buscar" aria-label="Search">
      <button class="btn-carrito" type="submit">Buscar</button>
    </form>
    <div style="margin-right: 30px">
      <button class="btn-carrito"> Carrito<i class="fa-solid fa-cart-shopping"></i> <span id="contador-carrito">0</span> </button>
    </div>
  </div>
</template>

<style>
.container-gral {
  display: flex;
  width: 100%;
  height: 100px;
  justify-content: space-between;
  align-items: center;
  background-color: papayawhip;
  box-shadow: 2px 2px 2px 1px rgba(0, 0, 0, 0.2);
}
.btn-carrito {
  width: 100px;
  height: 30px;
  font-family: 'Comfortaa', cursive;
  font-weight: 700;
  color: #ffffff;
  background-color: fuchsia;
  border: none;
  border-radius: 8px;
}
.input{
  width: 300px;
  height: 30px;
  border: 1px solid fuchsia;
  border-radius: 8px;
  text-align: center;
  margin-right: 10px;
}
</style>