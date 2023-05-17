<!-- eslint-plugin-vue -->
<template>
  <div>
    <div
      id="skill"
      class="text-center inline-block mt-16 py-16"
      style="margin-top: 200px !important"
    >
      <h1>Skill</h1>
    </div>
    <v-row>
      <v-col cols="12" sm="6">
        <h1>Profesional Skills</h1>
        <p>

        </p>

        <div
          class="orange d-flex justify-space-between"
          style="
            width: 100%;
            height: 40px;
            align-items: center;
            border-radius: 5px;
          "
        >
          <div class="d-flex">
            <v-icon>mdi-language-html5</v-icon>
            <h3>HTML5</h3>
          </div>
          <div>
            <h2 class="mx-6">25%</h2>
          </div>
        </div>

        <div
          class="light-blue d-flex justify-space-between"
          style="
            width: 100%;
            height: 40px;
            align-items: center;
            border-radius: 5px;
          "
        >
          <div class="d-flex">
            <v-icon>mdi-language-css3</v-icon>
            <h3>CSS3</h3>
          </div>
          <div>
            <h2 class="mx-6">30%</h2>
          </div>
        </div>

        <div
          class="amber d-flex justify-space-between"
          style="
            width: 100%;
            height: 40px;
            align-items: center;
            border-radius: 5px;
          "
        >
          <div class="d-flex">
            <v-icon>mdi-language-javascript</v-icon>
            <h3>JavaScript</h3>
          </div>
          <div>
            <h2 class="mx-6">1%</h2>
          </div>
        </div>

        <div
          class="green accent-4 d-flex justify-space-between"
          style="
            width: 100%;
            height: 40px;
            align-items: center;
            border-radius: 5px;
          "
        >
          <div class="d-flex">
            <v-icon>mdi-vuejs</v-icon>
            <h3>Vue</h3>
          </div>
          <div>
            <h2 class="mx-6">2%</h2>
          </div>
        </div>
      </v-col>
      <v-col cols="6"> </v-col>
    </v-row>
  </div>
</template>
