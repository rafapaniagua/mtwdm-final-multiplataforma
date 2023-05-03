<template>
  <article>
    <div class="card card-item">
      <img :src="cardItem.imagen" class="card-img-top">
      <div class="card-body">
        <h5 class="card-title">{{cardItem.descripcion}}</h5>
        <p class="card-text">${{cardItem.precio}}</p>
      </div>
    </div>
  </article>
</template>

<script>
export default {
  props: {
    cardItem: {
      type: Object,
      required: true
    }
  }
}
</script>

<style>

</style>