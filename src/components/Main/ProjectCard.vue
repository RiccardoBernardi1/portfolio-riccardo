<template>
  <div class="card m-3">
    <slot name="image"></slot>
    <div class="card-body">
      <h5 class="card-title fs-4 fw-bold"><slot></slot></h5>
      <p class="card-text fs-5">
        <slot name="description"></slot>
      </p>
      <a :href="link" class="btn btn-primary fw-bold me-3">Apri</a>
      <a :href="gitLink" class="btn btn-primary fw-bold">Apri su github</a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    link: String,
    gitLink: String,
  },
};
</script>

<style lang="scss" scoped>
.card-body {
  background-color: rgba($color: #1af3c4, $alpha: 0.3);
}
h5 {
  color: #3f167cdb;
}
a {
  color: bisque;
}
</style>
