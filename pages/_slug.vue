<template>
  <div class="grid grid-cols-1">
    <img src="~/assets/img/modelo_404.png" class="mx-auto" alt="" />
    <h1 class="text-center my-5">Erro 404 - Page {{ $route.path }} not found</h1>
  </div>
</template>
<script>
export default {
  transition: 'slide-bottom'
}
</script>
