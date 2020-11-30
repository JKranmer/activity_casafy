<template>
  <div class="bg-gray-100 rounded shadow-lg mb-5 md:mx-5 xl:mx-0">
    <p class="p-4 mt-10">
      <span class="font-bold uppercase">crowding found</span><br />
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nihil architecto
      nostrum asperiores eaque aliquid ad temporibus cumque commodi voluptates
      facilis minus totam harum, assumenda quasi iure illo? Earum, enim harum
    </p>
    <p class="p-4">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nihil architecto
      nostrum asperiores eaque aliquid ad temporibus cumque commodi voluptates
      facilis minus totam harum, assumenda quasi iure illo? Earum, enim harum.
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas assumenda
      quae dignissimos sit voluptate. Numquam dolorum at quam ex, dolore, totam
      qui quidem sed officiis eaque est eius repellendus quos.
    </p>
    <ul class="p-4 space-y-4">
      <li v-for="person in people" :key="person.name" class="grid grid-cols-3">
        <div
          class="rounded-full flex items-center justify-center w-12 h-12 bg-center bg-cover"
          :style="'background-image: url(' + person.img +');'"
        ></div>
        <span class="self-center"> {{ person.name }} </span>
        <b class="self-center"> {{ person.value }} </b>
      </li>
    </ul>
    <a
      href="#more"
      target="_blank"
      rel="noopener noreferrer"
      class="button--green mb-4"
    >
      More
    </a>
  </div>
</template>
<script>
export default {
  data () {
    return {
      people:
        [
          { name: 'Allan Frederic', img: 'https://image.freepik.com/fotos-gratis/foto-de-um-homem-pensativo-isolada-sobre-uma-parede-branca_295783-1405.jpg', value: '$123' },
          { name: 'David Smith', img: 'https://image.freepik.com/fotos-gratis/retrato-de-um-jovem-feliz-de-barba-vermelha-com-a-boca-escancarada-de-surpresa-vestindo-uma-camiseta-azul-apontando-o-dedo-para-copiar-o-espaco-no-lado-direito-isolado-sobre-o-fundo-rosa_295783-2871.jpg', value: '$173' },
          { name: 'Issac Polo', img: 'https://image.freepik.com/fotos-gratis/homem-atordoado-le-mensagem-de-texto-com-expressao-de-surpresa-segura-o-celular-e-descobre-algo-chocante_273609-17337.jpg', value: '$253' },
          { name: 'Sarah Walkers', img: 'https://image.freepik.com/fotos-gratis/retrato-de-uma-linda-garota-pensativa_171337-2554.jpg', value: '$839' }
        ]
    }
  }
}
</script>
