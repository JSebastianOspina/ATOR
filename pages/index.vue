<template>
  <div class="overflow-hidden scrollme">
    <MenuPrincipal class="mt-2" />
    <Sliderr class="md:mb-10" />

    <div class="md:flex md:flex-col md:justify-center md:items-center">
      <div class="mx-5 md:w-4/5">
        <Fundadores class="mt-3" />
        <Vision class="mx-2 p-3 mt-12" />
        <Mision class="mx-2 p-3 mt-20" />
      </div>
      <DondeEstamos class="mt-12" id="dondeestamos"/>

      <Comite2 class="px-5 sm:px-0" />

      <ParallaxBox />

      <VisitasInternacionales />

      <CharlasCursos class="px-5 sm:px-0" />

      <div class="mx-5 md:w-4/5"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
html{
  scroll-behavior: smooth;
}

</style>