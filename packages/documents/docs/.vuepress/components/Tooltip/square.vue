<template>
  <div class="center">
    <vs-tooltip square>
      <vs-button square flat>
        Do hover here
      </vs-button>
      <template #tooltip>
        This is a beautiful button
      </template>
    </vs-tooltip>
  </div>
</template>

<style scoped lang="scss">
.vs-button {
  margin: 0px;
}
</style>

