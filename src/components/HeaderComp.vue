<template>
  <q-header
    elevated
    reveal
    class="header flex no-wrap bg-white items-center justify-around"
  >
    <div name="icons non-selectable" class="flex" style="gap: 10px">
      <router-link to="/"
        ><q-img style="width: 200px" src="img/STELK LOGO.png"></q-img
      ></router-link>
    </div>

    <div class="flex cursor-pointer row no-wrap" style="gap: 50px">
      <div class="header-dropdown text-black">
        <div class="header-dropdown-title text-weight-medium">
          JALUR PENDAFTARAN <span class="material-icons">expand_more</span>
        </div>
        <div
          class="non-selectable header-dropdown-content absolute"
          style="padding-top: 20px"
        >
          <div class="bg-red-9 q-pa-sm" style="width: 150px">
            <a href="#bwh" class="q-pa-sm text-white text-weight-medium"
              >KEBAWAH</a
            >
            <router-link
              to="/login"
              class="q-pa-sm text-white text-weight-medium"
              >LOGIN</router-link
            >
          </div>
        </div>
      </div>

      <div class="header-dropdown text-black">
        <div class="header-dropdown-title text-weight-medium">
          JADWAL <span class="material-icons">expand_more</span>
        </div>
        <div
          class="non-selectable header-dropdown-content absolute"
          style="padding-top: 20px"
        >
          <div class="bg-red-9 q-pa-sm" style="width: 150px">
            <a href="#bwh" class="q-pa-sm text-white text-weight-medium"
              >KEBAWAH</a
            >
            <router-link
              to="/login"
              class="q-pa-sm text-white text-weight-medium"
              >LOGIN</router-link
            >
          </div>
        </div>
      </div>

      <div class="header-dropdown text-black">
        <div class="header-dropdown-title text-weight-medium">
          PROFIL JURUSAN <span class="material-icons">expand_more</span>
        </div>
        <div
          class="non-selectable header-dropdown-content absolute"
          style="padding-top: 20px"
        >
          <div class="bg-red-9 q-pa-sm" style="width: 150px">
            <a href="#bwh" class="q-pa-sm text-white text-weight-medium"
              >KEBAWAH</a
            >
            <router-link
              to="/login"
              class="q-pa-sm text-white text-weight-medium"
              >LOGIN</router-link
            >
          </div>
        </div>
      </div>

      <div class="header-dropdown text-black">
        <div class="header-dropdown-title text-weight-medium">
          HUBUNGI KAMI <span class="material-icons">expand_more</span>
        </div>
        <div
          class="non-selectable header-dropdown-content absolute"
          style="padding-top: 20px"
        >
          <div class="bg-red-9 q-pa-sm" style="width: 150px">
            <a href="#bwh" class="q-pa-sm text-white text-weight-medium"
              >KEBAWAH</a
            >
            <router-link
              to="/login"
              class="q-pa-sm text-white text-weight-medium"
              >LOGIN</router-link
            >
          </div>
        </div>
      </div>
      <div
        name="links"
        class="header-link flex non-selectable"
        style="gap: 10px"
      >
        <router-link
          v-if="!eventbus.loggedIn"
          to="/login"
          class="header-link text-weight-medium"
        >
          LOGIN
        </router-link>
        <router-link
        @click="updateEventBusValue"
          v-if="eventbus.loggedIn"
          to="/"
          class="header-link text-weight-medium"
        >
          KELUAR
        </router-link>
      </div>
    </div>
  </q-header>
</template>

<style>
.header {
  max-height: 70px;
}
.header-link:hover {
  color: #e91313;
}

.header-dropdown-title,
.header-dropdown a,
.header-link a,
.header-dropdown-content {
  transition: 0.2s ease;
}

.header-dropdown a,
.header-link a {
  text-decoration: none;
  color: rgb(0, 0, 0);
}

.header-dropdown-content {
  display: none;
}

.header-dropdown:hover .header-dropdown-content {
  display: block;
}

.header-dropdown-content a {
  display: block;
}

.header-dropdown-content a:hover {
  color: rgb(255, 185, 185) !important;
}

.header-dropdown:hover .header-dropdown-title {
  color: #e91313 !important;
}
</style>

<script>
import eventbus from "@/js/eventbus.js";

export default {
  data() {
    return {
      eventbus: eventbus,
    };
  },
  methods: {
    updateEventBusValue() {
      eventbus.loggedIn.value = false;
    },
  },
};
</script>
