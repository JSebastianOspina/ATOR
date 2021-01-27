<template>
  <div class="flex flex-col justify-center items-center w-full pb-10 fondo">
    <h2 class="text-center text-3xl font-bold my-12">
      Estructura organizacional
    </h2>
    <div
      class="border-double border-4 p-2 border-grey-400 w-full md:w-2/4 mb-6"
      v-for="(i, key) in data"
      :key="key"
    >
      <h3 class="text-2xl parrafo font-bold text-center">
        {{ i.nombre }}
      </h3>
      <h4 class="text-lg parrafo text-center mb-2">Enero 2020 – Enero 2021</h4>
      <ul class="parrafo ml-2">
        <li v-for="(o, llave) in i.miembros" :key="o.Cargo">
          <strong>{{ o.Cargo }}</strong>
          <ul>
            <li v-for="(u, llave2) in o.persona" :key="llave2">
              {{ u }}
            </li>
          </ul>
        </li>
      </ul>
    </div>

    <h2 class="text-center text-3xl font-bold mt-4 mb-6">
      Ponencias e Investigaciones
    </h2>
    <div
      class="border-double border-4 p-2 border-grey-400 w-full md:w-2/4 mb-6"
     
    >
      <h3 class="parrafo font-bold text-center mb-4">
      <a href="https://link.springer.com/chapter/10.1007%2F978-3-030-49076-8_4">XII Conferencia Mexicana, MCPR 2020, Morelia, México, 24–27 de junio de 2020</a>
      </h3>
      <h3 class="parrafo font-bold text-center">
      <a href="https://sfo-asso.fr/wp-content/uploads/2019/01/140.pdf">XVIII Conferencia Europea de Orquideologia .Paris - Francia</a>
      </h3>
    </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      data: [
        {
          nombre: "Junta directiva",
          miembros: [
            {
              Cargo: "Presidente",
              persona: ["Jaime Arturo Campo"],
            },
            {
              Cargo: "Vice-presidente",
              persona: ["Carlos Eduardo Beltran "],
            },
            {
              Cargo: "Secretaria",
              persona: ["Luz Patricia Naranjo"],
            },
            {
              Cargo: "Tesorero",
              persona: ["Luis Fernando Arias"],
            },
            {
              Cargo: "Vocal 1",
              persona: ["Cesar Augusto Nuñez"],
            },
            {
              Cargo: "Vocal 2",
              persona: ["Manuel Guillermo Forero"],
            },
            {
              Cargo: "Vocal 3",
              persona: ["Marco Rada"],
            },
            {
              Cargo: "Revisor Fiscal",
              persona: ["Sandra Liliana Riveros"],
            },
            {
              Cargo: "Asesor Jurídico",
              persona: ["Juan Manuel Barrero"],
            },
          ],
        },
        {
          nombre: "Comité Científico",
          miembros: [
            {
              Cargo: "Prof Dr Marco rada ph.D",
              persona: [
                "director comite cientifico",
                "Investigador ATO e Investigador Asociado, Laboratoio de Anfibios",
                "Instituto de Biociências, Universidade de São Paulo (USP), Brasil.",
              ],
            },
            {
              Cargo: "Prof Dr. Luz Patricia Naranjo Ph.D",
              persona: ["G. Naturatu /Fac. de Ciencias Universidad de Ibagué."],
            },
            {
              Cargo: "Prof Dr.Manuel Guillermo Forero .Ph.D",
              persona: [
                "Director de investigacion D + Tec / ",
                "Decano Fac. de Ingeniería Universidad de Ibagué.",
              ],
            },
            {
              Cargo: "Prof/Cand PhD. Miguel Cesar Moreno ",
              persona: [
                "Representate de Naturatu,",
                " Asesor programa Biologia Ambiental (Fac. de Ciencias Unibague).",
              ],
            },
            {
              Cargo: "Prof. Cesar Augusto Nuñez MSc ",
              persona: [
                "Asesor CORTOLIMA ",
                "Asesor línea ambiental Facultad de Ciencias Universidad.de Ibagué",
                "Asesor ATO.",
              ],
            },
          ],
        },

        {
          nombre: "Comité Laboratoios y Biotecnología",
          miembros: [
            {
              Cargo: "Ing Juan Carlos Otavo MSc ",
              persona: ["Coordinador."],
            },
            {
              Cargo: "Yensi Katherine Moreno.",
              persona: [
                "Tec / Asistente laboratoio de Biotecnología e Invitro/ Universidad de Ibagué.",
              ],
            },
          ],
        },
        {
          nombre: "Comité de Eventos",
          miembros: [
            {
              persona: ["La junta Directiva y todos los Asociados de la ATO "],
            },
          ],
        },
      ],
    };
  },
};
</script>

<style>
.fondo {
  background-color: #faf6f5;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='88' height='24' viewBox='0 0 88 24'%3E%3Cg fill-rule='evenodd'%3E%3Cg id='autumn' fill='%23eae6e5' fill-opacity='0.4'%3E%3Cpath d='M10 0l30 15 2 1V2.18A10 10 0 0 0 41.76 0H39.7a8 8 0 0 1 .3 2.18v10.58L14.47 0H10zm31.76 24a10 10 0 0 0-5.29-6.76L4 1 2 0v13.82a10 10 0 0 0 5.53 8.94L10 24h4.47l-6.05-3.02A8 8 0 0 1 4 13.82V3.24l31.58 15.78A8 8 0 0 1 39.7 24h2.06zM78 24l2.47-1.24A10 10 0 0 0 86 13.82V0l-2 1-32.47 16.24A10 10 0 0 0 46.24 24h2.06a8 8 0 0 1 4.12-4.98L84 3.24v10.58a8 8 0 0 1-4.42 7.16L73.53 24H78zm0-24L48 15l-2 1V2.18A10 10 0 0 1 46.24 0h2.06a8 8 0 0 0-.3 2.18v10.58L73.53 0H78z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
}
.parrafo {
  color: #4f4f4f;
  line-height: 1.65em;
}
</style>