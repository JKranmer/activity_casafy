<template>
  <div class="grid grid-rows">
    <div class="grid xl:grid-cols-5 grid-cols-1 m-5 gap-4">
      <div class="xl:col-span-4 grid xl:grid-cols-4 md:grid-cols-2 grid-cols-1 gap-4">
        <div class="bg-yellow-500 md:col-span-2 xl:col-span-1">
          <img
            class="rounded-t-sm"
            src="https://picsum.photos/seed/picsum/500/700"
            alt="logo_1"
          />
        </div>
        <div class="bg-yellow-500 xl:col-span-3 md:col-span-2">
          <iframe
            width="100%"
            height="500"
            src="https://www.youtube.com/embed/fZl6ufxmAqI"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
        <Card />
        <Card />
        <Card />
        <Card />
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
