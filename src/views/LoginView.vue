<template>
  <q-layout view="lHh Lpr lFf">
    <q-page class="flex">
      <img
        src="img\STELK LOGO.png"
        alt=""
        class="absolute"
        style="right: 30px; max-width: 250px"
      />
      <img
        src="img\wave.png"
        alt=""
        class="absolute fit"
        style="max-width: 50%"
      />
      <img
        src="img\Siswa stelk.png"
        alt=""
        class="absolute q-ma-lg"
        style="max-width: 50%; bottom: 5%"
      />

      <q-card
        rounded-border
        class="q-pa-md flex column justify-end absolute"
        style="
          min-width: 350px;
          top: 30%;
          min-height: 380px;
          right: 10%;
          gap: 20px;
        "
      >
        <q-img
          src="img\Sehati.png"
          class="absolute-center z-top"
          style="width: 150px; top: 0"
        ></q-img>

        <q-card-section class="q-pt-none flex column">
          <q-input color="red-8" v-model="email" label="Email"></q-input>

          <q-input
            class="text-subtitle"
            color="red-8"
            v-model="password"
            label="Password"
          >
          </q-input
          >
        </q-card-section>
        <q-card-section>
          <router-link to="/"
            ><q-btn
              elevated
              style="border-radius: 8px"
              color="red-8"
              rounded
              size="md"
              label="Masuk"
              no-caps
              class="full-width"
              @click="updateEventBusValue"
            ></q-btn
          ></router-link>
          <div class="text-center text-grey q-mt-sm text-caption">
            Powered by SMK Telkom Makassar
          </div>
        </q-card-section>
      </q-card>
    </q-page>
  </q-layout>
</template>

<script>
import { ref } from "vue";
import eventbus from "@/js/eventbus.js";

export default {
  setup() {
    return {
      email: ref(""),
      password: ref(""),
    };
  },
  methods: {
    updateEventBusValue() {
      eventbus.loggedIn.value = true;
    },
  },
};
</script>

<style>
.margin00 {
  margin-top: 5px;
}

.text00 {
  font-size: 15px;
  margin-top: 15px;
}

.my_card {
  width: 600px;
}

.serif {
  font-family: serif;
}

.bg-image {
  background-image: url(D:\projeksmk\ujianreal\public\img\wave.png);
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
