<template>
  <v-row id="home">
    <v-col cols="12" sm="6">
      <div
        class="d-flex align-center"
        style="margin-top: 100px; font-size: 30px"
      >
        <h1 class="text-h4 text-sm-h1 font-weight-bold">
          Hi,<br />
          I'am <span class="pink--text">Yah Lee</span><br />
          back end developer
        </h1>
      </div>

      <div>
        <v-btn class="pink white--text my-15 " x-large> Contact </v-btn>
        <div>
          <a
            class="mr-4 text-decoration-none"
            href="https://web.facebook.com/kuamuag.hlub.106"
            target="_blank"
            ><v-icon large>mdi-facebook</v-icon></a
          >
          <a
            class="mr-4 text-decoration-none"
            href="https://github.com/Yah-lee"
            target="_blank"
            ><v-icon large>mdi-github</v-icon></a
          >
          <a
            class="text-decoration-none"
            href="https://wa.me/8562093819369"
            target="_blank"
            ><v-icon large>mdi-whatsapp</v-icon></a
          >
        </div>
      </div>
    </v-col>
    <v-col cols="12" sm="6" class="d-flex justify-center align-center py-6">
      <div class="home__img">
        <svg
          class="home__blob mt-16"
          viewBox="0 0 479 467"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
        >
          <mask id="mask0" mask-type="alpha">
            <path
              d="M9.19024 145.964C34.0253 76.5814 114.865 54.7299 184.111 29.4823C245.804 6.98884 311.86 -14.9503 370.735 14.143C431.207 44.026 467.948 107.508 477.191 174.311C485.897 237.229 454.931 294.377 416.506 344.954C373.74 401.245 326.068 462.801 255.442 466.189C179.416 469.835 111.552 422.137 65.1576 361.805C17.4835 299.81 -17.1617 219.583 9.19024 145.964Z"
            />
          </mask>
          <g mask="url(#mask0)">
            <path
              d="M9.19024 145.964C34.0253 76.5814 114.865 54.7299 184.111 29.4823C245.804 6.98884 311.86 -14.9503 370.735 14.143C431.207 44.026 467.948 107.508 477.191 174.311C485.897 237.229 454.931 294.377 416.506 344.954C373.74 401.245 326.068 462.801 255.442 466.189C179.416 469.835 111.552 422.137 65.1576 361.805C17.4835 299.81 -17.1617 219.583 9.19024 145.964Z"
            />
            <image class="home__blob-img" x="40" y="55" href="/profile2.png" />
          </g>
        </svg>
        <br />
        <div class="text-center">
          <div class="text-p pink-text font-weight-bold">How many stars will you give me </div>
          <v-rating
            v-model="rating"
            icon-label="custom icon label text {0} of {1}"
          ></v-rating>
        </div>
      </div>
    </v-col>
  </v-row>
</template>
<script>
export default {
  data() {
    return {
      rating: 0,
    };
  },
};
</script>
