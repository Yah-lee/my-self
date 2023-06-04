<template>
  <v-app>
    <!-- <v-navigation-drawer v-model="drawer" fixed temporary>
      <h1 v-for="item in list" :key="item">{{ item.text }}</h1>
    </v-navigation-drawer>
    <Header :list="list" @openDrawer="drawer = true" /> -->

    <!-- <v-navigation-drawer v-model="drawer" fixed temporary right>
      <h1 v-for="item in list" :key="item">{{ item.text }}</h1>
    </v-navigation-drawer>
    <Header :list="list" @openDrawer="drawer = true" /> -->

    <v-navigation-drawer
      class="font-weight-bold text-h4 py-16 mt-50 text-center black"
      v-model="drawer"
      fixed
      temporary
      right
      width="200"
    >
      <a
        v-for="item in list"
        :key="item.id"
        class=" pink--text font-weight-bold text-decoration-none txt "
        :href="`#${item.id}`"
      >
        {{ item.text }}
      </a>
    </v-navigation-drawer>
    <Header :list="list" @openDrawer="drawer = true" />

    <!-- <v-navigation-drawer v-model="drawer" fixed temporary right>
  <v-list color="text--blue">
    <v-list-item v-for="item in list" :key="item">{{ item.text }}</v-list-item>
  </v-list>
</v-navigation-drawer>
 -->

    <!-- 
 <v-navigation-drawer v-model="drawer" fixed temporary right>
  <v-list class="red--text">
    <v-list-item v-for="item in list" :key="item">{{ item.text }}</v-list-item>
  </v-list>
</v-navigation-drawer>
 -->

    <v-container>
      <Home />
      <About />
      <myskill />
      <!-- Skill -->

      <div>
        <div id="skill" class="text-center inline-block mt-16 py-16">
          <h1 class="">Skill</h1>
        </div>
        <v-row>
          <v-col cols="12" sm="6">
            <h1 class="pink--text font-weight-bold">Profesional Skills</h1>

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
                <h2 class="mx-6">10%</h2>
              </div>
            </div>

            <div
              class="light-blue d-flex justify-space-between mt-4"
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
                <h2 class="mx-6">15%</h2>
              </div>
            </div>

            <div
              class="amber d-flex justify-space-between mt-4"
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
              class="green accent-4 d-flex justify-space-between mt-4"
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

      <!-- Skill -->

      <!-- work -->

      <div id="work" class="text-center inline-block mt-10 py-16">
        <h1>Work</h1>
      </div>
      <v-row>
        <v-col cols="12" sm="3"
          >I am a person who is positive about every aspect of life. There are
          many things I like to do, to see, and to experience. I like to read, I
          like to write; I like to think, I like to dream; I like to talk, I
          like to listen. I like to see the sunrise in the morning, I like to
          see the moonlight at night; I like to feel the music flowing on my
          face, I like to smell the wind coming from the ocean. I like to look
          at the clouds in the sky with a blank mind, I like to do thought
          experiment when I cannot sleep in the middle of the night. I like
          flowers in spring, rain in summer, leaves in autumn, and snow in
          winter. I like to sleep early, I like to get up late; I like to be
          alone, I like to be surrounded by people. I like country’s peace, I
          like metropolis’ noise; I like the beautiful west lake in Hangzhou, I
          like the flat cornfield in Champaign. I like delicious food and
          comfortable shoes; I like good books and romantic movies. I like the
          land and the nature, I like people. And, I like to laugh.</v-col
        >
        <v-col v-col cols="12" sm="3"
          >I am a person who is positive about every aspect of life. There are
          many things I like to do, to see, and to experience. I like to read, I
          like to write; I like to think, I like to dream; I like to talk, I
          like to listen. I like to see the sunrise in the morning, I like to
          see the moonlight at night; I like to feel the music flowing on my
          face, I like to smell the wind coming from the ocean. I like to look
          at the clouds in the sky with a blank mind, I like to do thought
          experiment when I cannot sleep in the middle of the night. I like
          flowers in spring, rain in summer, leaves in autumn, and snow in
          winter. I like to sleep early, I like to get up late; I like to be
          alone, I like to be surrounded by people. I like country’s peace, I
          like metropolis’ noise; I like the beautiful west lake in Hangzhou, I
          like the flat cornfield in Champaign. I like delicious food and
          comfortable shoes; I like good books and romantic movies. I like the
          land and the nature, I like people. And, I like to laugh.</v-col
        >
        <v-col v-col cols="12" sm="3"
          >I am a person who is positive about every aspect of life. There are
          many things I like to do, to see, and to experience. I like to read, I
          like to write; I like to think, I like to dream; I like to talk, I
          like to listen. I like to see the sunrise in the morning, I like to
          see the moonlight at night; I like to feel the music flowing on my
          face, I like to smell the wind coming from the ocean. I like to look
          at the clouds in the sky with a blank mind, I like to do thought
          experiment when I cannot sleep in the middle of the night. I like
          flowers in spring, rain in summer, leaves in autumn, and snow in
          winter. I like to sleep early, I like to get up late; I like to be
          alone, I like to be surrounded by people. I like country’s peace, I
          like metropolis’ noise; I like the beautiful west lake in Hangzhou, I
          like the flat cornfield in Champaign. I like delicious food and
          comfortable shoes; I like good books and romantic movies. I like the
          land and the nature, I like people. And, I like to laugh.</v-col
        >
        <v-col v-col cols="12" sm="3"
          >I am a person who is positive about every aspect of life. There are
          many things I like to do, to see, and to experience. I like to read, I
          like to write; I like to think, I like to dream; I like to talk, I
          like to listen. I like to see the sunrise in the morning, I like to
          see the moonlight at night; I like to feel the music flowing on my
          face, I like to smell the wind coming from the ocean. I like to look
          at the clouds in the sky with a blank mind, I like to do thought
          experiment when I cannot sleep in the middle of the night. I like
          flowers in spring, rain in summer, leaves in autumn, and snow in
          winter. I like to sleep early, I like to get up late; I like to be
          alone, I like to be surrounded by people. I like country’s peace, I
          like metropolis’ noise; I like the beautiful west lake in Hangzhou, I
          like the flat cornfield in Champaign. I like delicious food and
          comfortable shoes; I like good books and romantic movies. I like the
          land and the nature, I like people. And, I like to laugh.</v-col
        >
      </v-row>

      <!-- work -->

      <!-- contact -->
      <div
        id="contact"
        class="text-center inline-block mt-16"
        style="margin-top: 200px !important"
      >
        <h1>Contact</h1>
      </div>
      <template>
        <v-form v-model="valid">
          <v-container>
            <v-row>
              <v-col cols="12" md="4">
                <v-text-field
                  v-model="firstname"
                  :rules="nameRules"
                  :counter="10"
                  label="First name"
                  required
                ></v-text-field>
              </v-col>

              <v-col cols="12" md="4">
                <v-text-field
                  v-model="email"
                  :rules="nameRules"
                  :counter="100"
                  label="E-mail"
                  required
                ></v-text-field>
              </v-col>

              <v-col cols="12" md="4">
                <v-text-field
                  v-model="comments"
                  :rules="emailRules"
                  label="Comments"
                  required
                ></v-text-field>
              </v-col>
            </v-row>
          </v-container>
        </v-form>
      </template>

      <!-- contact -->
    </v-container>
  </v-app>
</template>
<script>
import MySkill from "../components/MySkill.Vue";

export default {
  data() {
    return {
      valid: false,
      firstname: "",
      email: "",
      comments: "",
      nameRules: [(v) => !!v || "", (v) => v.length <= 100 || ""],
      emailRules: [(v) => !!v || " "],
      drawer: false,
      list: [
        {
          text: "Home",
          id: "home",
        },
        {
          text: "About",
          id: "about",
        },
        {
          text: "Skill",
          id: "skill",
        },
        {
          text: "Work",
          id: "work",
        },
        {
          text: "Contact",
          id: "contact",
        },
      ],
    };
  },
  components: { MySkill },
};
</script>
