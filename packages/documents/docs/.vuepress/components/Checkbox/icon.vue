<template>
  <div class="center checks">
    <vs-checkbox v-model="option1">
      <template #icon>
        <i class="bx bx-check"></i>
      </template>
    </vs-checkbox>
    <vs-checkbox success v-model="option2">
      <template #icon>
        <i class="bx bx-check-double"></i>
      </template>
    </vs-checkbox>
    <vs-checkbox danger v-model="option3">
      <template #icon>
        <i class="bx bx-x"></i>
      </template>
    </vs-checkbox>
    <vs-checkbox warn v-model="option4">
      <template #icon>
        <i class="bx bxs-shield"></i>
      </template>
    </vs-checkbox>
    <vs-checkbox dark v-model="option5">
      <template #icon>
        <i class="bx bxs-heart"></i>
      </template>
    </vs-checkbox>
    <vs-checkbox color="#7d33ff" v-model="option6">
      <template #icon>
        <i class="bx bx-brightness"></i>
      </template>
    </vs-checkbox>
    <vs-checkbox color="rgb(59,222,200)" v-model="option7">
      <template #icon>
        <i class="bx bxs-paint"></i>
      </template>
    </vs-checkbox>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";

const option1 = ref(true);
const option2 = ref(true);
const option3 = ref(true);
const option4 = ref(true);
const option5 = ref(true);
const option6 = ref(true);
const option7 = ref(true);
</script>
<style lang="scss">
.checks {
  .vs-checkbox-content {
    margin: 5px;
  }
}
</style>
