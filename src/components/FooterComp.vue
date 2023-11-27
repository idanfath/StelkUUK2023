<template>
  <q-layout
    view="lHh Lpr lFf"
    class="bg-white text-black flex justify-center items-center"
    style="min-height: auto"
  >
    <div class="flex no-wrap justify-center q-ma-lg">
      <div class="menu-utama q-mx-xl" style="width: 350px">
        <div class="text-h6 q-my-sm">Tentang Kami</div>
        <div class="text-grey q-mb-sm text-grey-6">
          <span class="text-black text-weight-medium">
            SMK Telkom Makassar
          </span>
          Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s
        </div>
      </div>

      <div class="hubungi-kami q-mx-xl" style="width: 350px">
        <div class="text-h6 q-my-sm">Lokasi Kami</div>
        <div class="text-grey">
          <a
            href="https://maps.google.com/"
            class="q-mb-sm text-grey-6 routerlink-hover"
            style="text-decoration: none"
          >
            Jalan Lorem Kelurahan Ipsum Lorem Ipsum is simply dummy
          </a>
        </div>
      </div>

      <div class="bg-transparent text-left q-mx-xl" style="width: auto">
        <div class="text-h6 q-my-sm">Sosial Media Kami</div>
        <div class="flex row no-wrap" style="gap: 5px;">
          <a href="https://facebook.com">
            <q-icon name="facebook" size="30px" color="red-9"></q-icon>
          </a>
          <a href="https://instagram.com">
            <q-icon name="facebook" size="30px" color="red-9"></q-icon>
          </a>

        </div>
      </div>
    </div>
  </q-layout>
  <q-layout
    view="lHh Lpr lFf"
    class="bg-red-8 text-white flex justify-center items-center"
    style="min-height: auto"
  >
    <div class="text-caption1 text-grey-3 text-center q-pa-lg">
      <div>
        Copyright @2023
        <span class="text-white"> SMK Telkom Makassar </span>
      </div>
    </div>
  </q-layout>
</template>

<script>
export default {};
</script>

<style>
.footercomp {
  background-color: white;
}

.routerlink-hover:hover {
  transition: 0.2s ease;
  color: #696969 !important;
}
</style>
