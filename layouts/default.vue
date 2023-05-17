<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" fixed temporary>
      <h1 v-for="item in list" :key="item">{{ item.text }}</h1>
    </v-navigation-drawer>
    <Header :list="list" @openDrawer="drawer = true" />
    <v-container>
      <Home />
      <About />
      <!-- <TestPage /> -->
      <div
        id="work"
        class="text-center inline-block mt-16 py-16"
        style="margin-top: 200px !important"
      >
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
    </v-container>
  </v-app>
</template>
<script>
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
          text: "Homes",
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
};
</script>
