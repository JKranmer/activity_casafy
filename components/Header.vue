<template>
  <div class="grid grid-cols-1 sm:grid-cols-2 bg-gradient-to-br from-blue-800 to-blue-500">
    <div class="mx-auto sm:m-auto"><img src="~/assets/img/logo_polo.png" class="p-10 sm:px-10" alt="1" style="width:100%;" ></div>
    <div class="mb-4 sm:my-4">
      <div class="rounded-l-lg shadow-md text-center bg-gray-200 grid md:grid-cols-2 grid-cols-1">
        <form class="text-left ml-4 ">
          <input class="border-2 border-green-600 px-4 align-top mt-2 border-solid bg-gray-200 border">
          <button class="pt-3">
            <svg xmlns="http://www.w3.org/2000/svg" class="opacity-50 p-1 w-6 m-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" /></svg>
          </button>
        </form>
        <ul class="grid grid-cols-3 sm:pt-3 p-3">
          <li class="mx-auto"><a href="#" title="Filter"><img src="https://www.flaticon.com/svg/static/icons/svg/1312/1312139.svg" width="23px"></a></li>
          <li class="mx-auto"><a href="#" title="Notification"><img src="https://www.flaticon.com/svg/static/icons/svg/1312/1312142.svg" width="23px" alt=""></a></li>
          <li class="mx-auto"><a href="#" title="User"><img src="https://www.flaticon.com/svg/static/icons/svg/185/185983.svg" width="23px" alt=""></a></li>
        </ul>
      </div>
      <ul class="rounded-l-lg shadow-md text-center gap-4 py-3 my-6 bg-gray-200 grid grid-cols-3">
        <li><a href="#" title="Spanish" class="group rounded-md text-gray-500 inline-flex items-center text-base font-medium hover:text-gray-900 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-900"><img src="~/assets/img/spanish-language.svg" alt="" class="h-6"></a></li>
        <li><a href="#" title="Chinese"  class="group rounded-md text-gray-500 inline-flex items-center text-base font-medium hover:text-gray-900 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-900"><img src="~/assets/img/chinese-language.svg" alt="" class="h-6"></a></li>
        <li><a href="#" title="English" class="group rounded-md text-gray-500 inline-flex items-center text-base font-medium hover:text-gray-900 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-900"><img src="~/assets/img/english-language.svg" alt="" class="h-6"></a></li>
      </ul>
    </div>
  </div>
</template>
