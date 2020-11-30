<template>
  <div
    class="grid sm:grid-cols-5 grid-cols-1 shadow-md gap-4 py-6 mb-6 bg-gray-200"
  >
    <div class="sm:col-span-1 hidden sm:block"></div>
    <nav class="sm:col-span-4">
      <ul class="grid-cols-4 grid text-center">
        <li>
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about">About</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/store">Store</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/contact">Contact</NuxtLink>
        </li>
      </ul>
    </nav>
  </div>
</template>
