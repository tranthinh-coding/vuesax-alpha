<template>
  <div class="center">
    <vs-button
      shadow
      icon
      @click="openNotification(null, null, `<i class='bx bxs-time'></i>`)"
    >
      <i class="bx bx-border-radius b-r"></i> 
      <i class="bx bxs-time"></i>
    </vs-button>
    <vs-button
      flat
      icon
      @click="openNotification(null, 'primary', `<i class='bx bxs-user-pin'></i>`)"
    >
      <i class="bx bx-border-radius b-r"></i> 
      <i class="bx bxs-user-pin"></i>
    </vs-button>
    <vs-button
      flat
      success
      icon
      @click="openNotification(
        'top-right',
        'success',
        `<i class='bx bx-select-multiple' ></i>`
      )"
    >
      <i class="bx bx-border-radius t-r"></i>
      <i class="bx bx-select-multiple"></i>
    </vs-button>
    <vs-button
      flat
      danger
      icon
      @click="openNotification('top-left', 'danger', `<i class='bx bxs-bug'></i>`)"
    >
      <i class="bx bx-border-radius t-l"></i> 
      <i class="bx bxs-bug"></i>
    </vs-button>
    <vs-button
      flat
      warn
      icon
      @click="openNotification('bottom-left', 'warn', `<i class='bx bx-error' ></i>`)"
    >
      <i class="bx bx-border-radius b-l"></i> 
      <i class="bx bx-error"></i>
    </vs-button>
    <vs-button
      flat
      dark
      icon
      @click="openNotification(
        'bottom-center',
        'dark',
        `<i class='bx bx-folder-open'></i>`
      )"
    >
      <i class="bx bx-border-bottom"></i>
      <i class="bx bx-folder-open"></i>
    </vs-button>
    <vs-button
      flat
      color="#7d33ff"
      icon
      @click="
        openNotification('top-center', '#7d33ff', `<i class='bx bx-bell' ></i>`)
      "
    >
      <i class="bx bx-border-top"></i>
      <i class="bx bx-bell"></i>
    </vs-button>
    <vs-button
      flat
      color="rgb(59,222,200)"
      icon
      @click="openNotification(
        null,
        'rgb(59,222,200)',
        `<i class='bx bx-calendar' ></i>`
      )"
    >
      <i class="bx bx-border-radius b-r"></i>
      <i class="bx bx-calendar"></i>
    </vs-button>
  </div>
</template>

<script lang="ts" setup>
import { notification } from "vuesax-alpha";

const openNotification = (position = null, color, icon) => {
  notification({
    icon,
    color,
    position,
    title: "Documentation Vuesax-alpha",
    text: "These documents refer to the latest version of Vuesax-alpha, to see the documents of the previous versions you can do it here ???? Vuesax4.0",
  });
};
</script>

<style scoped lang="scss">
.vs-button {
  margin: 10px;
}
i {
  margin: 2px;
  font-size: 1.2rem;
  transform-origin: center;
  &.b-r {
    transform: rotate(90deg);
  }
  &.t-r {
    transform: rotate(0deg);
  }
  &.t-l {
    transform: rotate(-90deg);
  }
  &.b-l {
    transform: rotate(-180deg);
  }
}
</style>
