<template>
  <v-app>
    <v-container>
      <div class="d-flex justify-space-between">
      <div>
      <h1>Yah Lee</h1>
    </div>
    <div class="d-flex align-center">
      <a 
      v-for="item in list"
      :key="item"
      href=""
      class="text-decoration-none mr-5 grey--text font-weight-bold"
      >
      {{ item }}
    </a>
    </div>
  </div>
    </v-container>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      list: ["Home", "About", "Skill", "Work", "Contact"],
    };
  },
};
</script>
