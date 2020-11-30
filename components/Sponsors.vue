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
          { name: 'Nike', logo: 'https://logospng.org/download/nike/logo-nike-1536.png', link: '/sponsor1', class: 'self-center', styleImg: 'max-height:100px; margin:auto; filter: invert(1) ' },
          { name: 'Adidas', logo: 'https://i.pinimg.com/originals/fe/52/81/fe52814e2f2de9cd68c5c048b7d32e2c.png', link: '/sponsor2', class: 'self-center max-h-2', styleImg: 'max-height:100px; margin:auto; filter: invert(1)' },
          { name: 'Lupo', logo: 'https://upload.wikimedia.org/wikipedia/commons/thumb/2/25/Lupo_logo.svg/1280px-Lupo_logo.svg.png', link: '/sponsor4', class: 'self-center', styleImg: 'max-height:100px; margin:auto; filter: invert(1); ' },
          { name: 'Puma', logo: 'https://i.pinimg.com/originals/d6/2e/e2/d62ee237e901fb9d16b7714b9bd165bb.png', link: '/sponsor3', class: 'self-center', styleImg: 'max-height:100px; margin:auto; filter: invert(1) ' },
          { name: 'Ralpgh Lauren', logo: 'https://logos-world.net/wp-content/uploads/2020/04/Ralph-Lauren-Symbol.png', link: '/sponsor5', class: 'hidden sm:block self-center', styleImg: 'max-height:100px; margin:auto; filter: invert(1) ' }
        ],
      title: 'TESTE'
    }
  }
}
</script>
