<template>
  <div class="center">
    <vs-tooltip>
      <vs-button shadow> Default </vs-button>
      <template #tooltip> This is a beautiful button </template>
    </vs-tooltip>
    <vs-tooltip color="primary">
      <vs-button flat> Primary </vs-button>
      <template #tooltip> This is a beautiful button </template>
    </vs-tooltip>
    <vs-tooltip color="success">
      <vs-button success flat> Success </vs-button>
      <template #tooltip> This is a beautiful button </template>
    </vs-tooltip>
    <vs-tooltip color="danger">
      <vs-button danger flat> Danger </vs-button>
      <template #tooltip> This is a beautiful button </template>
    </vs-tooltip>
    <vs-tooltip color="warn">
      <vs-button warn flat> Warning </vs-button>
      <template #tooltip> This is a beautiful button </template>
    </vs-tooltip>
    <vs-tooltip color="dark">
      <vs-button dark flat> Dark </vs-button>
      <template #tooltip> This is a beautiful button </template>
    </vs-tooltip>
    <vs-tooltip color="#7d33ff">
      <vs-button color="#7d33ff" flat> HEX </vs-button>
      <template #tooltip> This is a beautiful button </template>
    </vs-tooltip>
    <vs-tooltip color="rgb(59,222,200)">
      <vs-button color="rgb(59,222,200)" flat> RGB </vs-button>
      <template #tooltip> This is a beautiful button </template>
    </vs-tooltip>
  </div>
</template>

<style scoped lang="scss">
.vs-button {
  margin: 0px;
}
.vs-tooltip-content {
  margin: 5px;
}
</style>
