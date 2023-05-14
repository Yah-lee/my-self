<template>
  <v-app>
    <div class="black" style="position: fixed; width: 100%; z-index:100;">
      <v-container class="d-flex justify-space-between">
        <div>
          <h1>Yah Lee</h1>
        </div>
        <div class="d-flex align-center">
          <a v-for="item in list" :key="item.id" :href="`#${item.id}`"
            class="text-decoration-none mr-10 white--text font-weight-bold">
            {{ item.text }}
          </a>
        </div>
      </v-container>
    </div>
    <v-container>
      <v-row>
        <v-col cols="6">
          <div class="d-flex align-center" style="margin-top: 100px; font-size: 30px">
            <h1>
              Hi,<br />
              I'am <span class="pink--text">Yah Lee</span><br />
              back end developer
            </h1>
          </div>
          <div class="">
            <v-btn class="pink white--text my-15" x-large> Contact </v-btn>
            <div>
              <a class="mr-4" href="https://web.facebook.com/kuamuag.hlub.106" target="_blank"><v-icon
                  large>mdi-facebook</v-icon></a>
              <a class="mr-4" href="https://github.com/Yah-lee" target="_blank"><v-icon large>mdi-github</v-icon></a>
              <a href="https://wa.me/8562093819369" target="_blank"><v-icon large>mdi-whatsapp</v-icon></a>
            </div>
          </div>
        </v-col>
        <v-col cols="6">
          <div class="home__img">
            <svg class="home__blob" viewBox="0 0 479 467" xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink">
              <mask id="mask0" mask-type="alpha">
                <path
                  d="M9.19024 145.964C34.0253 76.5814 114.865 54.7299 184.111 29.4823C245.804 6.98884 311.86 -14.9503 370.735 14.143C431.207 44.026 467.948 107.508 477.191 174.311C485.897 237.229 454.931 294.377 416.506 344.954C373.74 401.245 326.068 462.801 255.442 466.189C179.416 469.835 111.552 422.137 65.1576 361.805C17.4835 299.81 -17.1617 219.583 9.19024 145.964Z" />
              </mask>
              <g mask="url(#mask0)">
                <path
                  d="M9.19024 145.964C34.0253 76.5814 114.865 54.7299 184.111 29.4823C245.804 6.98884 311.86 -14.9503 370.735 14.143C431.207 44.026 467.948 107.508 477.191 174.311C485.897 237.229 454.931 294.377 416.506 344.954C373.74 401.245 326.068 462.801 255.442 466.189C179.416 469.835 111.552 422.137 65.1576 361.805C17.4835 299.81 -17.1617 219.583 9.19024 145.964Z" />
                <image class="home__blob-img" x="40" y="55" href="/profile2.png" />
              </g>
            </svg>
          </div>
        </v-col>
      </v-row>
      <div id="about" class="text-center inline-block mt-16" style="margin-top: 200px !important">
        <h1>About</h1>
      </div>
      <v-row>
        <v-col v-col cols="6">

        </v-col>
        <v-col v-col cols="6">
          <div class="mt-16">
            <h4>I am a person who is positive about every aspect of life. There are many things I like to do, to see, and
              to experience. I like to read, I like to write; I like to think, I like to dream; I like to talk, I like to
              listen. I like to see the sunrise in the morning, I like to see the moonlight at night; I like to feel the
              music flowing on my face, I like to smell the wind coming from the ocean. I like to look at the clouds in
              the sky with a blank mind, I like to do thought experiment when I cannot sleep in the middle of the night. I
              like flowers in spring, rain in summer, leaves in autumn, and snow in winter. I like to sleep early, I like
              to get up late; I like to be alone, I like to be surrounded by people. I like country’s peace, I like
              metropolis’ noise; I like the beautiful west lake in Hangzhou, I like the flat cornfield in Champaign. I
              like delicious food and comfortable shoes; I like good books and romantic movies. I like the land and the
              nature, I like people. And, I like to laugh.</h4>
          </div>
        </v-col>
      </v-row>
      <div id="Skill" class="text-center inline-block mt-16" style="margin-top: 200px !important">
        <h1>Skill</h1>
      </div>
      <v-row>
        <v-col v-col cols="5">
          <h1>Profesional Skills</h1>
          <p>I am a person who is positive about every aspect of life. There are many things I like to do, to see, and
              to experience. I like to read, I like to write; I like to think, I like to dream; I like to talk, I like to
              listen. I like to see the sunrise in the morning, I like to see the moonlight at night; I like to feel the
              music flowing on my face, I like to smell the wind coming from the ocean. I like to look at the clouds in
              the sky with a blank mind, I like to do thought experiment when I cannot sleep in the middle of the night. I
              like flowers in spring, rain in summer, leaves in autumn, and snow in winter. I like to sleep early, I like
              to get up late; I like to be alone, I like to be surrounded by people. I like country’s peace, I like
              metropolis’ noise; I like the beautiful west lake in Hangzhou, I like the flat cornfield in Champaign. I
              like delicious food and comfortable shoes; I like good books and romantic movies. I like the land and the
              nature, I like people. And, I like to laugh.</p>

              <div class="orange d-flex justify-space-between" style="width: 100%; height:40px; align-items: center;  border-radius:5px ;"> <div class="d-flex"> <v-icon>mdi-language-html5</v-icon><h3>HTML5</h3></div>
              <div><h2 class="mx-6">25%</h2></div>
              </div>
              <br/>
              <div class="light-blue d-flex justify-space-between" style="width: 100%; height:40px; align-items: center;  border-radius:5px ;"> <div class="d-flex"> <v-icon>mdi-language-css3</v-icon><h3>CSS3</h3></div>
              <div><h2 class="mx-6">30%</h2></div>
              </div>
              <br/>
              <div class="amber d-flex justify-space-between" style="width: 100%; height:40px; align-items: center;  border-radius:5px ;"> <div class="d-flex"> <v-icon>mdi-language-javascript</v-icon><h3>JavaScript</h3></div>
              <div><h2 class="mx-6">1%</h2></div>
              </div>
              <br/>
              <div class="green accent-4 d-flex justify-space-between" style="width: 100%; height:40px; align-items: center;  border-radius:5px ;"> <div class="d-flex"> <v-icon>mdi-vuejs</v-icon><h3>Vue</h3></div>
              <div><h2 class="mx-6">2%</h2></div>
              </div>
        </v-col>
        <v-col v-col cols="6">
          
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
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
};
</script>
