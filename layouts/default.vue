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
      class="text-decoration-none mr-10 grey--text font-weight-bold"
      >
      {{ item }}
    </a>
    </div>
  </div>

  <nuxt/>

  <v-row>
    <v-col cols="6">
      <div class=" d-flex align-center justify-center" style="margin-top: 100px; font-size: 30px;">
        <h1>Hi,<br> I'am <span>Yah Lee</span><br> back end developer</h1>
      </div>
    </v-col>
    <v-col cols="6">
        <v-img src="https://www.pixelstalk.net/wp-content/uploads/2016/08/Best-Amazing-Images-For-Desktop.jpg" style="background-color: black;
      width: 400px;
      height: 400px;
      margin-top:100px;
      margin-left: 150px;
      border-top-left-radius: 500px;
      border-top-right-radius: 400px;
      border-bottom-left-radius: 350px;
      border-bottom-right-radius: 600px;"></v-img>
      </v-avatar>
        </v-col>
  </v-row>

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
