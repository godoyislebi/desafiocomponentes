<template>
  <div>
    <ul class="list-group text-start">
      <li class="list-group-item bg-none tipograph-rick">
        <img class="img-circle" :src="datos.image" :alt="datos.name" />
        <h2 class="d-inline-block">{{ datos.name }}</h2>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ListaRick",
  props: {
    datos: {
      type: Object,
      default: () => {},
    },
  },
};
</script>

<style></style>
