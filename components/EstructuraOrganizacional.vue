<template>
  <div class="mt-6">
    <div>
      <h2 class="text-3xl">Estructura organizacional</h2>
      <p class="text-justify mt-4 parrafo">
        La Asociación se rige a través de los siguientes órganos: Asamblea
        General, Junta Directiva y Presidente. La Asamblea General está
        constituida por las personas que tengan el aval de asociados
        conservacionistas y / o investigadores. A lo cual se accedé, por
        invitación (membresía). La Junta Directiva está constituida por: un
        presidente, un vicepresidente, un secretario, un tesorero y tres vocales
        La Asociación tiene un Revisor Fiscal y un asesor jurídico. La
        Asociación cuenta con un comité científico y un comité de laboratorio
        (biotecnología), con carácter asesor de la presidencia de la ATO.
      </p>
    </div>
    <div class="border-dotted border-4 border-red-200 p-1 mt-6 externo">
      <slider
        animation="fade"
        :interval="40000"
        :speed="1000"
        :control-btn="false"
        height="380px"
      >
        <slider-item>
          <div
            class="flex flex-col justify-center items-center h-full w-full bg-cover bg-center"
            style="background-image: url(junta-directiva.jpeg)"
          >
          <div id="overlay">

          </div>
            <div class="z-10">
                <h1 class="text-2xl text-gray-200 font-bold text-center">Junta directiva</h1>
                <h2 class="text-xl text-gray-200 text-center mb-2">
                  Enero 2020 – Enero 2021
                </h2>
                <ul class="text-gray-200 ml-2">
                  <li><strong>Presidente</strong>: Jaime Arturo Campo</li>
                  <li>
                    <strong>Vice-presidente</strong>: Carlos Eduardo Beltran Reyes
                  </li>
                  <li><strong>Secretaria</strong>: Luz Patricia Naranjo</li>
                  <li><strong>Tesorero</strong>: Luis Fernando Arias</li>
                  <li><strong>Vocal 1</strong>: Cesar Augusto Nuñez</li>
                  <li><strong>Vocal 2</strong>: Manuel Guillermo Forero</li>
                  <li><strong>Vocal 3</strong>: Marco Rada</li>
                  <li><strong>Revisor Fiscal</strong>: Sandra Liliana Riveros</li>
                  <li><strong>Asesor Jurídico</strong>: Juan Manuel Barrero</li>
                </ul>
            </div>
          </div>
        </slider-item>

       <slider-item>
          <div
            class="flex flex-col justify-center items-center h-full w-full bg-cover bg-center"
            style="background-image: url(junta-directiva.jpeg)"
          >
          <div id="overlay">

          </div>
            <div class="z-10">
                <h1 class="text-2xl text-gray-200 font-bold text-center">Comité Científico</h1>
            
                <ul class="text-gray-200 ml-2">
                  <li><strong>Prof Dr Marco Rada Ph.D</strong>: Jaime Arturo Campo</li>
                  <li>
                    <strong>Vice-presidente</strong>: Carlos Eduardo Beltran Reyes
                  </li>
                  <li><strong>Secretaria</strong>: Luz Patricia Naranjo</li>
                  <li><strong>Tesorero</strong>: Luis Fernando Arias</li>
                  <li><strong>Vocal 1</strong>: Cesar Augusto Nuñez</li>
                  <li><strong>Vocal 2</strong>: Manuel Guillermo Forero</li>
                  <li><strong>Vocal 3</strong>: Marco Rada</li>
                  <li><strong>Revisor Fiscal</strong>: Sandra Liliana Riveros</li>
                  <li><strong>Asesor Jurídico</strong>: Juan Manuel Barrero</li>
                </ul>
            </div>
          </div>
        </slider-item>
      </slider>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.parrafo {
  color: #4f4f4f;
  line-height: 1.65em;
}
#overlay {
  position: absolute; /* Sit on top of the page content */
  width: 100%; /* Full width (cover the whole page) */
  height: 100%; /* Full height (cover the whole page) */
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0,0,0,0.3); /* Black background with opacity */
  z-index: 2; /* Specify a stack order in case you're using a different order for other elements */
  cursor: pointer; /* Add a pointer on hover */
}
</style>