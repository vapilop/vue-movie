<script setup>
import Search from "./Search.vue";
import HeartIcon from "./icons/HeartIcon.vue";
</script>
<template>
  <div class="flex justify-between items-center">
    <router-link to="/">
      <h1
        class="text-xl font-semibold tracking-wider text-gray-200 md:text-2xl"
      >
        Фильмы
      </h1>
    </router-link>

    <router-link
      to="/fav"
      class="flex text-red-600 items-center cursor-pointer"
    >
      <HeartIcon />

      <span class="text-lg tracking-wide md:text-xl">Любимые фильмы</span>
    </router-link>
    <img src="https://images.unsplash.com/photo-1673337615896-a849cef919e2?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzfHx8ZW58MHx8fHw%3D&auto=format&fit=crop&w=500&q=60" class="rounded-full w-32" alt="Avatar"/>

  </div>
  <p
    class="
      mt-6
      mb-7
      text-gray-200 text-xs
      font-light
      tracking-wide
      md:text-lg md:tracking-wider
      lg:text-sm
    "
  >
    Ты можешь найти, что посмотреть сегодня вечером
  </p>
  <div class="inline-flex shadow-md hover:shadow-lg focus:shadow-lg" role="group">
    <button type="button" class="rounded-l inline-block px-6 py-2.5 bg-yellow-500 text-white font-medium text-xs leading-tight uppercase hover:bg-yellow-600 focus:bg-yellow-600 focus:outline-none focus:ring-0 active:bg-yellow-700 transition duration-150 ease-in-out">min рейтинг</button>
    <button type="button" class="inline-block px-6 py-2.5 bg-yellow-500 text-white font-medium text-xs leading-tight uppercase hover:bg-yellow-600 focus:bg-yellow-600 focus:outline-none focus:ring-0 active:bg-yellow-700 transition duration-150 ease-in-out">новые</button>
    <button type="button" class="rounded-r inline-block px-6 py-2.5 bg-yellow-500 text-white font-medium text-xs leading-tight uppercase hover:bg-yellow-600 focus:bg-yellow-600 focus:outline-none focus:ring-0 active:bg-yellow-700 transition duration-150 ease-in-out">max рейтинг</button>
  </div>
</template>