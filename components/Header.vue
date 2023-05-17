<template>
  <div class="black" style="position: fixed; width: 100%; z-index: 2">
    <v-container class="d-flex justify-space-between">
      <div>
        <h1>Yah Lee</h1>
      </div>
      <div v-if="$vuetify.breakpoint.xs">
        <v-icon @click="$emit('openDrawer')">mdi-menu</v-icon>
      </div>
      <div v-else class="d-flex align-center">
        <a
          v-for="item in list"
          :key="item.id"
          :href="`#${item.id}`"
          class="text-decoration-none mr-10 white--text font-weight-bold"
        >
          {{ item.text }}
        </a>
      </div>
    </v-container>
  </div>
</template>
<script>
export default {
  props: {
    list: {
      type: Array,
      default: () => {},
    },
  },
};
</script>
