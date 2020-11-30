<template>
  <div class="bg-gray-100 rounded shadow-lg m-5">
    <img
      class="rounded-t-sm"
      :src="card.img"
      :alt="card.title"
    />
    <p class="p-4">
      <span class="font-bold">{{card.title}}</span><br />
      {{card.text}}
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
</template>
