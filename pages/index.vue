<template>
  <div class="grid grid-rows">
    <div class="grid xl:grid-cols-5 grid-cols-1 m-5 gap-4">
      <div
        class="xl:col-span-4 grid xl:grid-cols-4 md:grid-cols-2 grid-cols-1 gap-4"
      >
        <div class="md:col-span-2 xl:col-span-1">
          <img
            class="rounded-t-sm hidden xl:block 2xl:hidden"
            src="https://picsum.photos/id/1033/700/1150"
            alt="logo_1"
          />
          <img
            class="rounded-t-sm block xl:hidden"
            src="https://picsum.photos/id/1033/1300/500"
            alt="logo_1"
          />
        </div>
        <div class="xl:col-span-3 md:col-span-2">
          <iframe
            width="100%"
            height="100%"
            style="min-height:200px;"
            src="https://www.youtube.com/embed/fZl6ufxmAqI"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
        <!-- <Card  v-for="card in cards" :key="card.title"/> -->
        <div
          v-for="card in cards"
          :key="card.title"
          class="bg-gray-100 rounded shadow-lg m-5"
        >
          <img class="rounded-t-sm" :src="card.img" :alt="card.title" />
          <p class="p-4">
            <span class="font-bold">{{ card.title }}</span
            ><br />
            {{ card.text }}
          </p>
          <a
            :href="card.link"
            target="_blank"
            rel="noopener noreferrer"
            class="button--green mb-4 "
          >
            More
          </a>
        </div>
      </div>
      <Crowding />
    </div>
    <Sponsors class="mt-5" />
  </div>
</template>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

<script>
export default {
  head: {
    title: 'Home page',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'Home page description'
      }
    ]
  },
  data () {
    return {
      cards: [
        {
          title: 'Allan Frederic',
          img: 'https://picsum.photos/id/1015/500/200',
          text:
            'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry s standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.',
          link: '$123'
        },
        {
          title: 'David Smith',
          img: 'https://picsum.photos/id/1002/500/200',
          text:
            'It is a long established fact that a reader will be distracted by the readable will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, ',
          link: '$123'
        },
        {
          title: 'Issac Polo',
          img: 'https://picsum.photos/id/1/500/200',
          text:
            'Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text, and a search for lorem ipsum will uncover many web sites still in their  for lorem ipsum will uncover many web sites still infancy.',
          link: '$123'
        },
        {
          title: 'Sarah Walkers',
          img: 'https://picsum.photos/id/103/500/200',
          text:
            'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don t look even slightly believable. Humour, or randomised words which don t . ',
          link: '$123'
        }
      ]
    }
  }
}
</script>
