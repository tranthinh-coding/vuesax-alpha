<template>
  <div class="center">
    <vs-radio v-model="picked" val="1">
      Label
    </vs-radio>
    <vs-radio label-before v-model="picked" val="2">
      label Before
    </vs-radio>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";

const picked = ref(1);
</script>

<style lang="scss" scoped>
.center {
  flex-direction: column;
  align-items: flex-start;
  .vs-radio-content {
    margin: 5px 0px;
  }
}
</style>