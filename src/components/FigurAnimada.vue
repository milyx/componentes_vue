<template>
  <div>
    <div class="content d-flex flex-start">
      <img
        :src="lolito.image"
        :alt="lolito.name"
        width="100"
        height="auto"
        class="py-2 img"
      />
      <h3 class="py-5 px-2">
        {{ lolito.name }}
      </h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "FigurAnimada",
  props: {
    lolito: {
      type: Object,
      default: () => {},
    },
  },
};
</script>

<style>
.img {
  border-radius: 50%;
}
</style>
