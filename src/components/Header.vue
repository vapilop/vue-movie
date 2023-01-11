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
    <button class="bg-red-500 ...">
  Регистрация
</button>
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
  <fieldset>
  <legend>Год выпуска</legend>

  <input id="draft" class="peer/draft" type="radio" name="status" checked />
  <label for="draft" class="peer-checked/draft:text-white">max</label>

  <input id="published" class="peer/published" type="radio" name="status" />
  <label for="published" class="peer-checked/published:text-white">min</label>

</fieldset>
</template>