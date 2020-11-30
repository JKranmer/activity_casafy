<template>
  <div class="grid bg-gradient-to-b from-blue-500 to-blue-800 p-5 grid-cols-2 sm:grid-cols-5">
    <div v-for="sponsor in sponsors" :key="sponsor.name" :class="sponsor.class + ' m-3'"><a :title="sponsor.name" :href="sponsor.link" target="_blank" rel="noopener noreferrer"><img :src='sponsor.logo'  :style="sponsor.styleImg"  :alt="sponsor.name"></a> </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      sponsors:
        [
          { name: 'Nike', logo: '/img/nike.png', link: '/nike', class: 'self-center', styleImg: 'max-height:100px; margin:auto; filter: invert(1) ' },
          { name: 'Adidas', logo: '/img/adidas.png', link: '/adidas', class: 'self-center max-h-2', styleImg: 'max-height:100px; margin:auto; filter: invert(1)' },
          { name: 'Lupo', logo: '/img/lupo.png', link: '/lupo', class: 'self-center', styleImg: 'max-height:100px; margin:auto; filter: invert(1); ' },
          { name: 'Puma', logo: '/img/puma.png', link: '/puma', class: 'self-center', styleImg: 'max-height:100px; margin:auto; filter: invert(1) ' },
          { name: 'Ralpgh Lauren', logo: '/img/Ralph-Lauren-Symbol.png', link: '/ralph', class: 'hidden sm:block self-center', styleImg: 'max-height:100px; margin:auto; filter: invert(1) ' }
        ],
      title: 'TESTE'
    }
  }
}
</script>
