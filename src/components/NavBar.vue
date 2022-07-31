<template>
  <div class="container-gral shadow-sm p-3 mb-5 bg-body rounded">
    <a style="margin-left: 20px" class="navbar-brand" href="#">
      <img src="/docs/5.2/assets/brand/bootstrap-logo.svg" alt="" width="30" height="24">
    </a>
    <form class="d-flex" role="search">
      <input class="form-control me-2" type="search" placeholder="Buscar" aria-label="Search">
      <button class="btn btn-outline-success" type="submit">Buscar</button>
    </form>
    <div style="margin-right: 30px">
      <button>Carrito <span>(4)</span></button>
    </div>
  </div>
</template>

<style>
.container-gral {
  display: flex;
  width: 100%;
  height: 60px;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  background-color: papayawhip;
  margin-bottom: 20px;
}
</style>