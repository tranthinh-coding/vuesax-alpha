<template>
  <div class="center con-pagination">
    <vs-pagination circle v-model="page" :length="20" />
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";

const page = ref(1);
</script>

<style lang="scss">
.con-pagination {
  .vs-pagination-content {
    margin: 10px 0px;
  }
}
</style>
