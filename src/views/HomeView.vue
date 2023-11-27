<template>
  <q-layout id="top" class="non-selectable">
    <HeaderComp></HeaderComp>
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
    <div
      flat
      class="absolute-center flex justify-end text-dark text-center"
      style="width: 70%"
    >
      <div class="flex column">
        <div class="text-bold text-h4">THE REAL INFORMATICS SCHOOL</div>
        <div class="text-caption">
          Pelopor SMK bidang Teknologi Informasi dan Komunikasi di Indonesia.
        </div>
      </div>
    </div>
    <!-- <q-img
      class="absolute-bottom-right"
      src="https://media.tenor.com/cyORI7kwShQAAAAj/shigure-ui-dance.gif"
      style="width: 200px"
    /> -->
  </q-layout>

  <q-layout style="min-height: 1050px;">
    <div class="flex column items-center" style="gap: 100px">
      <div class="text-center" style="padding-top: 60px">
        <div class="text-bold text-h3">Jalur Pendaftaran</div>
        <div class="text-subtitle1">
          Berikut merupakan jalus pendaftaran yang kami tawarkan kepada calon
          pendaftar
        </div>
      </div>
      <div class="flex row justify-between items-center no-wrap" style="width: 70%">
        <div class="flex column" style="gap: 10px">
          <div class="text-bold text-h4">Jalur Prestasi Akademik</div>
          <div class="text-subtitle1">
            <div>Berikut merupakan persyaratan untuk jalur prestasi</div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Bidang prestasi meliputi Akademis dan Non-Akademis</div>
            </div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Harus jago</div>
            </div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Bisa menggokil</div>
            </div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Mengjago</div>
            </div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Siap ganti nickname</div>
            </div>
          </div>
        </div>
        <div>
          <img src="img\ilustrasi 1.png"/>
        </div>
      </div>

      <div class="flex row justify-between items-center no-wrap" style="width: 70%">
        <div>
          <img src="img\ilustrasi 2.png" />
        </div>
        <div class="flex column" style="gap: 10px">
          <div class="text-bold text-h4">Jalur Reguler</div>
          <div class="text-subtitle1">
            <div>Berikut merupakan persyaratan untuk jalur prestasi</div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Bidang prestasi meliputi Akademis dan Non-Akademis</div>
            </div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Harus jago</div>
            </div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Bisa menggokil</div>
            </div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Mengjago</div>
            </div>
            <div class="flex row items-center" style="gap: 5px">
              <q-icon name="check" color="red-8" />
              <div>Siap ganti nickname</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </q-layout>

  <q-layout style="min-height: 800px;">
    <div class="flex justify-center column items-center" style="margin-top: 50px;">
      <div class="text-bold text-h4">Jadwal Perisai</div>
      <div class="text-subtitle1">
        <div>Berikut merupakan jadwal untuk perisai</div>
      </div>
      <div class="flex row no-wrap justify-between q-pt-xl" style="width: 70%;" >
          <qCardComp></qCardComp>
          <qCardComp></qCardComp>
          <qCardComp></qCardComp>
      </div>
    </div>
  </q-layout>

  <q-layout id="bwh" style="min-height: 100px">
    <FooterComp></FooterComp>
  </q-layout>
</template>

<script>
// @ is an alias to /src
import HeaderComp from "@/components/HeaderComp.vue";
import FooterComp from "@/components/FooterComp.vue";
import qCardComp from "@/components/qCardComp.vue";

export default {
  components: {
    HeaderComp,
    FooterComp,
    qCardComp,
  },
};
</script>

<style>
body {
  font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif !important;
}
html {
  scroll-behavior: smooth;
}
.bg-image.homeview {
  background-image: url(https://i.ytimg.com/vi/yfw693T_eCY/maxresdefault.jpg);
  background-size: cover;
}

body {
  background-color: rgb(255, 255, 255);
}
</style>
