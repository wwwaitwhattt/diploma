<script>
export default {
  name: 'FormGrid',
}
</script>

<template>
  <div :class="$style.root">
    <div :class="$style.wrapper">

    </div>
  </div>
</template>

<style module lang="scss">
.root {
  width: 100%;
}

.wrapper {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);

  @include md {
    grid-template-rows: auto;
    grid-template-columns: minmax(0, 1fr);
  }
}
</style>
